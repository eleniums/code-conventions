# Go Style Guidelines
The conventions detailed here are as close to the official recommendations as possible. As always, consistency within a project or organization is more important than rigid adherence to these conventions.

Note:
- `PascalCase` variables, functions, and structs are, by definition, exported from the package (public).
- `camelCase` variables, functions, and structs are, by definition, not exported from the package (private).

## Structs
Use `PascalCase` (unless the struct is unexported):
```go
type SomeStruct struct {
    // ...
}
```

## Public Methods
Use `PascalCase` for method name and `camelCase` for parameters:
```go
func SomePublicMethod(someParameter int) {
    // ...
}
```

## Private Methods
Use `camelCase` for method name and `camelCase` for parameters:
```go
func somePrivateMethod(someParameter int) {
    // ...
}
```

## Public Fields
Use `PascalCase`:
```go
var SomePublicField int
```

## Private Fields
Use `camelCase`:
```go
var somePrivateField int
```

## Local Variables
Use `camelCase`:
```go
someLocalVariable := 1
someOtherLocalVariable := SomeMethod()
```

## Constant Variables
Use `PascalCase` or `camelCase`:
```go
const SomePublicConstant = 1
const somePrivateConstant = 1
```

## Interfaces
Use `PascalCase` (unless for some reason the interface is unexported):
```go
type Writer interface {
    // ...
}
```

## Packages
Lowercase and, if possible, a single word:
```go
package foobar
```

## Abbreviations and acronyms
Acronyms and initialisms should be all caps:
- `IOReader` or `ioReader`
- `HTMLButton` or `htmlButton`
- `ItemID` <- ID is an initialism, so it's always all caps

Abbreviations use `PascalCase` or `camelCase`:
- `WinSize` or `winSize`
- `CustOrder` or `custOrder`

## Brackets
Use "Egyptian" brackets:
```go
func EgyptianBrackets(someParameter int) {
    // ...
}
```

## Comments
Code comments should be formatted like so:
```go
// this is a code comment
```

Documentation comments should start with the variable, function, or struct name:
```go
// Foo is a function that does something.
func Foo(bar int) bool {
    // ...
}
```

## References
- https://golang.org/doc/effective_go.html
- https://github.com/uber-go/guide/blob/master/style.md
- https://github.com/golang/go/wiki/CodeReviewComments