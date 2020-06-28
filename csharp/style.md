# C# Style Guidelines

## Public Methods
Use `PascalCase`:
```
public void SomePublicMethod(int someParameter)
{
    ...
}
```

## Private Methods
Use `PascalCase`:
```
private void SomePrivateMethod(int someParameter)
{
    ...
}
```

## Public Fields
Use `PascalCase`:
```
public int SomePublicField = 1;
```

## Private Fields
Use `camelCase`:
```
private int somePrivateField = 1;
```

OR
```
private int _somePrivateField = 1;
```

Use `camelCase` with an underscore prefixed:

## Local Variables
Use `camelCase`:
```
int someLocalVariable = 1;
```

## Constant Variables
Use `PascalCase`:
```
const int SomeConstant = 1;
```

## References
- https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/identifier-names
- https://github.com/ktaranov/naming-convention/blob/master/C%23%20Coding%20Standards%20and%20Naming%20Conventions.md