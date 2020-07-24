# C# Style Guidelines
The conventions detailed here are as close as possible to the official recommendations. As always, consistency within a project or organization is more important than rigid adherence to these conventions.

## Classes
Use `PascalCase`:
```csharp
public class SomeClass
{
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
Use `camelCase`:
```csharp
int someLocalVariable = 1;
var someOtherLocalVariable = SomeMethod();
```

## Constant Variables
Use `PascalCase`:
```csharp
public const int SomeConstant = 1;
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
`Company.Product|Technology.Feature.Subnamespace`

## Abbreviations and acronyms
Capitalize acronyms that are two characters or fewer:
- `IOReader` or `ioReader`
- `HtmlButton` or `htmlButton`

Avoid abbreviations, but if necessary use `camelCase`:
- `GetWin`
- `ItemId`

## Brackets
Use vertically aligned brackets:
```csharp
public void VerticalBrackets(int someParameter)
{
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
public bool Foo(int bar)
{
    // ...
}
```

## References
- https://docs.microsoft.com/en-us/dotnet/standard/design-guidelines/naming-guidelines
- https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/language-specification/
- https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/identifier-names
- https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/coding-conventions
- https://github.com/ktaranov/naming-convention/blob/master/C%23%20Coding%20Standards%20and%20Naming%20Conventions.md