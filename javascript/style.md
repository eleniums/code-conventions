# JavaScript Style Guidelines
The conventions detailed here are as close as possible to the official recommendations. As always, consistency within a project or organization is more important than rigid adherence to these conventions.

## Classes
Use `PascalCase`:
```javascript
class SomeClass {
    constructor(foo, bar) {
        this.foo = foo;
        this.bar = bar;
    }
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
Use `camelCase` for method name and `camelCase` for parameters:
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

## Constants
Use all caps `SNAKE_CASE`:
```java
public static final int SOME_CONSTANT = 1;
```

## Enums
Use `PascalCase` for enum name and all caps `SNAKE_CASE` for enum values:
```java
public enum SomeEnum {
	SOME_ENUM_VALUE
}
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
```java
package com.company.subpackage;
```

NOTE: Package name should match directory structure.

## Abbreviations
Ignore casing of original words and use `PascalCase` or `camelCase` as appropriate:
- `IoReader` or `ioReader`
- `HtmlButton` or `htmlButton`
- `ItemId` or `itemId`

## Brackets
Use "Egyptian" brackets:
```java
public void egyptianBrackets(int someParameter) {
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
public int foo(int bar) {
    // ...
}
```

## References
- https://google.github.io/styleguide/jsguide.html
- https://www.robinwieruch.de/javascript-naming-conventions