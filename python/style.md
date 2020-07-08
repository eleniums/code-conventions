# Python Style Guidelines
The conventions detailed here are as close to the official recommendations as possible. As always, consistency within a project or organization is more important than rigid adherence to these conventions.

## Classes
Use `PascalCase`:
```python
class SomeClass:
    # ...
```

## Public Methods
Use `snake_case` for method name and `snake_case` for parameters:
```python
def some_public_method(some_parameter)
    # ...
```

## Private Methods
Use `snake_case` with a leading underscore for method name and `snake_case` for parameters:
```python
def _some_private_method(some_parameter):
    # ...
```

OR

Use `snake_case` with a double leading underscore (invokes name mangling - generally only use in classes designed to be subclassed):
```python
def __some_private_method(some_parameter):
    # ...
```

NOTE: This can technically be accessed with SomeClass._SomeClass__some_private_method

## Public Fields
Use `snake_case`:
```python
some_public_field = 1
```

## Private Fields
Use `snake_case` with a leading underscore (weak internal use indicator -  will not be imported by another package):
```python
_some_private_field = 1
```

OR

Use `snake_case` with a double leading underscore (invokes name mangling - generally only use in classes designed to be subclassed):
```python
__some_private_field = 1
```

NOTE: This can technically be accessed with SomeClass._SomeClass__some_private_field

## Local Variables
Use `snake_case`:
```python
some_local_variable = 1
some_other_local_variable = some_method()
```

## Constant Variables
Use all caps `SNAKE_CASE` (this is a convention as python does not have constants):
```python
SOME_CONSTANT = 1
```

## Abbreviations and acronyms
Capitalize acronyms if using `PascalCase`:
- `IOReader` or `ioReader`
- `HTMLButton` or `htmlButton`

All lowercase if using `snake_case`:
- `io_reader`
- `html_button`

## Comments
Code comments should be formatted like so:
```python
# This is a code comment.
```

Documentation comments should use the docstring format:
```python
def foo(bar):
    """Description of the method that fits in one line."""
    # ...
```

OR

```python
def foo(bar):
    """Description of the method that fits in one line.
    
    Add a more elaborate description here with parameters, etc.
    """
    # ...
```

## References
- https://www.python.org/dev/peps/pep-0008
- https://www.python.org/dev/peps/pep-0257
- https://visualgit.readthedocs.io/en/latest/pages/naming_convention.html