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
```javascript
class SomeClass {
    somePublicMethod(someParameter) {
        // ...
    }
}
```

## Private Methods
Use `camelCase` for method name with a leading underscore and `camelCase` for parameters:
```javascript
class SomeClass {
    _somePrivateMethod(someParameter) {
        // ...
    }
}
```

NOTE: The underscore is a convention that does not enforce private scoping. In [ES2019](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes/Private_class_fields), a hash prefix can be used to define a private method.
```javascript
class SomeClass {
    #somePrivateMethod(someParameter) {
        // ...
    }
}
```

## Public Fields
Use `camelCase`:
```javascript
class SomeClass {
    somePublicField = 1;
}
```

## Private Fields
Use `camelCase` with a leading underscore:
```javascript
class SomeClass {
    _somePrivateField = 1;
}
```

NOTE: The underscore is a convention that does not enforce private scoping. In [ES2019](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes/Private_class_fields), a hash prefix can be used to define a private field.
```javascript
class SomeClass {
    #somePrivateField = 1;
}
```

## Local Variables
Use `camelCase`:
```javascript
let someLocalVariable = 1;
let someOtherLocalVariable = someMethod();
```

## Constants
Use all caps `SNAKE_CASE`:
```javascript
const SOME_CONSTANT = 1;
```

## Abbreviations
Ignore casing of original words and use `PascalCase` or `camelCase` as appropriate:
- `IoReader` or `ioReader`
- `HtmlButton` or `htmlButton`
- `ItemId` or `itemId`

## Brackets
Use "Egyptian" brackets:
```javascript
function egyptianBrackets(someParameter) {
    // ...
}
```

## Comments
Code comments should be formatted like so:
```javascript
// This is a code comment.
```

Documentation comments should use the JSDoc format:
```javascript
/**
 * Description of the method.
 * @param {string} bar Description of parameter.
 * @returns {number} Description of return value.
 */
function foo(bar) {
    // ...
}
```

## References
- https://www.robinwieruch.de/javascript-naming-conventions
- https://google.github.io/styleguide/jsguide.html