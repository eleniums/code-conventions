# C# Style Guidelines

## Public Methods
Use `PascalCase`:
```csharp
public void SomePublicMethod(int someParameter)
{
    ...
}
```

## Private Methods
Use `PascalCase`:
```csharp
private void SomePrivateMethod(int someParameter)
{
    ...
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

## References
- https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/identifier-names
- https://github.com/ktaranov/naming-convention/blob/master/C%23%20Coding%20Standards%20and%20Naming%20Conventions.md