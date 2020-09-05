# Rust Style Guidelines
The conventions detailed here are as close as possible to the official recommendations. As always, consistency within a project or organization is more important than rigid adherence to these conventions.

## Structs
Use `PascalCase`:
```rust
struct SomeStruct {
    // ...
}
```

## Functions
Use `snake_case` for method name and `snake_case` for parameters:
```rust
fn some_function(some_parameter: i32) -> i32 {
    // ...
}
```

## Public Methods
Use `snake_case` for method name and `snake_case` for parameters:
```rust
impl SomeStruct {
    pub fn some_public_method(&self, some_parameter: i32) {
        // ...
    }
}
```

NOTE: `pub` exposes the method outside of the module.

## Private Methods
Use `snake_case` for method name and `snake_case` for parameters:
```rust
impl SomeStruct {
    fn some_private_method(&self, some_parameter: i32) {
        // ...
    }
}
```

NOTE: By default, methods and fields are only accessible to the module they belong to.

## Public Fields
Use `snake_case`:
```rust
struct SomeStruct {
    pub some_public_field: i32,
}
```

NOTE: `pub` exposes the field outside of the module.

## Private Fields
Use `snake_case`:
```rust
struct SomeStruct {
    some_private_field: i32,
}
```

NOTE: By default, methods and fields are only accessible to the module they belong to.

## Local Variables
Use `snake_case`:
```rust
let some_local_variable = 1;
let some_other_local_variable = some_method();
```

## Constants
Use all caps `SNAKE_CASE`:
```rust
const SOME_CONSTANT: i32 = 1;
```

## Enums
Use `PascalCase` for enum name and `PascalCase` for enum values:
```rust
enum SomeEnum {
	SomeEnumValue
}
```

## Interfaces
Interfaces should start with `I`:
```csharp
public interface IWriter
{
    // ...
}
```

## Brackets
Use "Egyptian" brackets:
```rust
fn egyptian_brackets(some_parameter: i32) {
    // ...
}
```

## Comments
Code comments should be formatted like so:
```rust
// This is a code comment.
```

Documentation comments should use triple slashes with the markdown format:
```rust
/// Description of the method.
/// 
/// Add a more elaborate description here that can span multiple lines.
/// 
/// # Arguments
/// 
/// * `bar` - Description of parameter.
/// 
/// # Return value
/// 
/// Description of return value.
fn foo(bar: i32) -> i32 {
    // ...
}
```

## References
- https://doc.rust-lang.org/1.0.0/style