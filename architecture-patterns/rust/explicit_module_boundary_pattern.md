# Explicit Module Boundary Pattern

## Overview
The **Explicit Module Boundary Pattern** (also called **Gateway Module Pattern**) is a Rust architectural pattern that uses `mod.rs` files as explicit gateways to control module boundaries and dependencies.

## Core Rules

### 1. Individual Module Files (Siblings)
- Each sibling module exports as `pub` what it needs to share with siblings OR the crate
- Individual files focus on their specific domain logic
- Use visibility modifiers to control access levels

### 2. Module Gateway (`mod.rs`)
The `mod.rs` file serves as the module's public contract:

```rust
// Bring all submodules into scope
mod submodule_a;
mod submodule_b;

// Internal-only exports (sibling access within this module)
use submodule_a::InternalType;

// Public exports (visible outside this module)
pub use submodule_a::{PublicType, public_function};
pub use submodule_b::{AnotherPublicType};
```

**The `mod.rs` defines the ENTIRE public interface** - if it's not in `mod.rs`, it's not public.

### 3. Import Patterns

| Context | Pattern | Example |
|---------|---------|---------|
| **Sibling to Sibling** | `super::sibling::Symbol` | `use super::auth::Credentials;` |
| **External Module** | `crate::module::Symbol` | `use crate::domain::AppUser;` |
| **Binary to Library** | `crate_name::module::Symbol` | `use myapp::domain::AppUser;` |

### 4. Visibility Levels

```rust
pub struct Public;           // Visible if re-exported in mod.rs
pub(crate) struct CrateWide; // Visible within entire crate
pub(super) struct ParentOnly; // Visible to parent module only
struct Private;              // Module-private only
```

## Benefits

1. **Explicit Dependencies** - All inter-module dependencies visible in `mod.rs`
2. **Controlled Boundaries** - Clear separation between public API and internals  
3. **Refactoring Safety** - Changes to internals don't break external consumers
4. **Complete Internal Refactoring Freedom** - Rename files, reorganize modules, move code around within a module without breaking any external code. Only need to update the `mod.rs` gateway, not hunt down imports throughout the codebase
5. **Documentation** - `mod.rs` serves as module documentation
6. **Layered Architecture** - Natural enforcement of architectural layers

## Example Structure

```
src/
├── domain/
│   ├── mod.rs          ← Gateway: defines public domain API
│   ├── user.rs         ← Sibling: user logic
│   ├── auth.rs         ← Sibling: auth logic  
│   └── cache.rs        ← Sibling: cache logic
├── repository/
│   ├── mod.rs          ← Gateway: defines public repository API
│   ├── user_repo.rs    ← Implementation
│   └── cache_repo.rs   ← Implementation
└── routes/
    ├── mod.rs          ← Gateway: defines public routes API
    └── user_routes.rs  ← Route handlers
```

## Anti-Patterns to Avoid

❌ **Bypassing the Gateway**
```rust
// DON'T: Direct access bypasses mod.rs contract
use crate::domain::user::UserInternal;
```

✅ **Use the Gateway**
```rust  
// DO: Access through public API
use crate::domain::User;
```

❌ **Leaky Abstractions**
```rust
// DON'T: Internal types in public signatures
pub fn get_user() -> InternalUserType { }
```

✅ **Clean Boundaries**
```rust
// DO: Only public types in public signatures  
pub fn get_user() -> User { }
```

## Implementation Checklist

- [ ] Each `mod.rs` has explicit `mod` declarations for all submodules
- [ ] Each `mod.rs` has clear separation of internal `use` vs public `pub use`
- [ ] Sibling modules import from each other using `super::` 
- [ ] External modules import through `crate::module::`
- [ ] No direct imports that bypass `mod.rs` gateways
- [ ] Public APIs only expose public types, never internals

## When to Use

✅ **Good for:**
- Multi-module applications
- Library crates with public APIs
- Projects requiring clear architectural boundaries
- Teams needing explicit dependency management

❌ **Overkill for:**
- Single-file applications  
- Prototypes
- Very simple projects with minimal modules

---

*Pattern Name: **Explicit Module Boundary Pattern** / **Gateway Module Pattern***
