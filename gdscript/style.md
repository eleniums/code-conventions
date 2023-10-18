# GDScript Style Guidelines
The conventions detailed here are as close as possible to the official recommendations. As always, consistency within a project or organization is more important than rigid adherence to these conventions.

## Classes
Use `PascalCase`:
```gdscript
class_name MyClass
```

NOTE: A file is a class, so this declaration is optional. Should save file as 'my_class.gd', although saving the file as 'MyClass.gd' is also acceptable.

## Functions
Use `snake_case` for function name and `snake_case` for parameters:
```gdscript
func some_function(some_parameter):
    # ...
```

NOTE: Prepend a single underscore (`_`) to virtual methods or private functions.

## Local Variables
Use `snake_case`:
```gdscript
var some_local_variable = 1
```

NOTE: Prepend a single underscore (`_`) to private variables.

## Constants
Use `CONSTANT_CASE`:
```gdscript
const SOME_CONSTANT = 1
```

## Enums
Use `PascalCase` for enum name and `CONSTANT_CASE` for enum values:
```gdscript
enum SomeEnum { SOME_ENUM_VALUE, ANOTHER_ENUM_VALUE }
```

## Abbreviations
Use `snake_case`:
- `io_reader`
- `html_button`
- `item_id`

## Comments
Code comments should be formatted like so:
```gdscript
# This is a code comment.
```

Documentation comments should start with a double `#`:
```gdscript
## Description of the function.
func foo(bar):
    # ...
```

## References
- https://docs.godotengine.org/en/stable/getting_started/scripting/gdscript/gdscript_styleguide.html
- https://docs.godotengine.org/en/stable/getting_started/scripting/gdscript/gdscript_basics.html#example-of-gdscript
- https://docs.godotengine.org/en/stable/tutorials/scripting/gdscript/gdscript_documentation_comments.html