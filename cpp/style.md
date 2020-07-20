# C++ Style Guidelines
The conventions detailed here are as close to the ISO C++ recommendations as possible. There are many accepted styles for C++ and not just one correct way of doing things. As always, consistency within a project or organization is more important than rigid adherence to these conventions.

## Classes
Use `snake_case`:
```cpp
class some_class {
    public:
        // ...
};
```

## Public Methods
Use `snake_case` for method name and `snake_case` for parameters:
```cpp
void some_public_method(int some_parameter)
{
    // ...
}
```

## Private Methods
Use `snake_case` for method name and `snake_case` for parameters:
```cpp
void some_private_method(int some_parameter)
{
    // ...
}
```

## Public Fields
Use `snake_case`:
```cpp
int some_public_field = 1;
```

## Private Fields
Use `snake_case`:
```cpp
int some_private_field = 1;
```

OR

Use `snake_case` with an underscore postfixed:
```cpp
int some_private_field_ = 1;
```

## Local Variables
Use `snake_case`:
```cpp
int some_local_variable = 1;
int some_other_local_variable = some_method();
```

## Constant Variables
Use `snake_case`:
```cpp
const int some_constant = 1;
```

## Macros
Use all caps `snake_case`:
```cpp
#define SOME_MACRO 1000
```

## Namespaces
Use `snake_case`:
```cpp
namespace some_namespace {
    // ...
}
```

## Abbreviations and acronyms
Use `snake_case`:
- `io_reader`
- `html_button`
- `item_id`

## Brackets
Use vertically aligned brackets for functions and "Egyptian" brackets for everything else (Stroustrup style):
```cpp
class egyptian_brackets_class {
    public:
        // ...
};

void vertical_brackets_function(int someParameter)
{
    if (egyptian_brackets_statement) {
        // ...
    }
}
```

## Comments
Code comments should be formatted like so:
```cpp
// this is a code comment
```

Documentation comments should use the Doxygen format:
```cpp
/*! \brief Description of the method.
    \param bar Description of parameter.
    \return Description of return value.
    
    A longer description of the method if needed.
*/
bool foo(int bar)
{
    // ...
}
```

## References
- https://github.com/isocpp/CppCoreGuidelines/blob/master/CppCoreGuidelines.md
- https://www.stroustrup.com/bs_faq2.html
- https://google.github.io/styleguide/cppguide.html
- https://github.com/lefticus/cppbestpractices/blob/master/03-Style.md