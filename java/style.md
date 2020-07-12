# Java Style Guidelines
The conventions detailed here are as close to the official recommendations as possible. As always, consistency within a project or organization is more important than rigid adherence to these conventions.

## Classes
Use `PascalCase`:
```java
public class SomeClass {
    // ...
}
```

## Public Methods
Use `camelCase` for method name and `camelCase` for parameters:
```java
public void somePublicMethod(int someParameter) {
    // ...
}
```

## Private Methods
Use `cascalCase` for method name and `camelCase` for parameters:
```java
private void somePrivateMethod(int someParameter) {
    // ...
}
```

## Public Fields
Use `camelCase`:
```java
public int somePublicField = 1;
```

## Private Fields
Use `camelCase`:
```java
private int somePrivateField = 1;
```

## Local Variables
Use `camelCase`:
```java
int someLocalVariable = 1;
int someOtherLocalVariable = SomeMethod();
```

## Constant Variables
Use all caps `SNAKE_CASE`:
```java
public static final int SOME_CONSTANT = 1;
```

## Interfaces
Use `PascalCase`:
```java
public interface Writer {
    // ...
}
```

## Packages
General rule for packages:
`com.company.subpackage`

NOTE: Package name should match directory structure.

## Abbreviations and acronyms
Ignore casing of original words and use `PascalCase` or `camelCase` as appropriate:
- `IoReader` or `ioReader`
- `HtmlButton` or `htmlButton`
- `ItemId` or `itemId`

## Brackets
Use "Egyptian" brackets:
```java
public void verticalBrackets(int someParameter) {
    // ...
}
```

## Comments
Code comments should be formatted like so:
```java
// This is a code comment.
```

Documentation comments should use the Javadoc format:
```java
/**
* Description of the method.
*
* @param bar Description of parameter.
* @return Description of return value.
*/
public bool foo(int bar) {
    // ...
}
```

## References
- https://www.oracle.com/java/technologies/javase/codeconventions-namingconventions.html
- https://www.javatpoint.com/java-naming-conventions
- https://www.geeksforgeeks.org/java-naming-conventions
- https://google.github.io/styleguide/javaguide.html
- https://www.tutorialspoint.com/java/java_documentation.htm