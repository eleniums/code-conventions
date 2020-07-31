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
Use `PascalCase` for method name and `camelCase` for parameters:
```csharp
public void SomePublicMethod(int someParameter)
{
    // ...
}
```

## Private Methods
Use `PascalCase` for method name and `camelCase` for parameters:
```csharp
private void SomePrivateMethod(int someParameter)
{
    // ...
}
```

## Public Fields
Use `PascalCase`:
```csharp
public int SomePublicField = 1;
```

## Private Fields
Use `camelCase`:
```csharp
private int somePrivateField = 1;
```

OR

Use `camelCase` with an underscore prefixed:
```csharp
private int _somePrivateField = 1;
```

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
```csharp
enum SomeEnum
{
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

## Namespaces
General rule for namespaces:
```csharp
namespace Company.Product
{
    // ...
}
```

OR

```csharp
namespace Technology.Feature.Subnamespace
{
    // ...
}
```

## Abbreviations
Capitalize acronyms that are two characters or fewer:
- `IOReader` or `ioReader`
- `HtmlButton` or `htmlButton`

Avoid abbreviations, but if necessary use `camelCase`:
- `GetWin`
- `ItemId`

## Brackets
Use "Egyptian" brackets:
```rust
fn egyptian_brackets(some_parameter: i32) {
    // ...
}
```

## Comments
Code comments should be formatted like so:
```csharp
// This is a code comment.
```

Documentation comments should use the xml format:
```csharp
/// <summary>
/// Description of the method.
/// </summary>
/// <param name="bar">Description of parameter.</param>
/// <returns>Description of return value.</returns>
public int foo(int bar)
{
    // ...
}
```

## References
- https://doc.rust-lang.org/1.0.0/style