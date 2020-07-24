# C Style Guidelines
The conventions detailed here are as close as possible to the Linux Kernel recommendations. There are many accepted styles for C and not just one correct way of doing things. As always, consistency within a project or organization is more important than rigid adherence to these conventions.

## Structs
Use `snake_case`:
```c
struct some_struct {
    /* ... */
};
```

## Functions
Use `snake_case` for function name and `snake_case` for parameters:
```c
void some_function(int some_parameter) {
    /* ... */
}
```

## Variables
Use `snake_case`:
```c
int some_variable = 1;
int some_other_variable = some_method();
```

## Constants
Use all caps `SNAKE_CASE`:
```c
const int SOME_CONSTANT = 1;
```

## Enums
Use `snake_case` for enum name and all caps `SNAKE_CASE` for enum values:
```c
enum some_enum {
	SOME_ENUM_VALUE
};
```

## Macros
Use all caps `SNAKE_CASE`:
```c
#define SOME_MACRO 1000
```

## Abbreviations
Use `snake_case`:
- `io_reader`
- `html_button`
- `item_id`

## Brackets
Use vertically aligned brackets for functions and "Egyptian" brackets for everything else (K&R style):
```c
struct egyptian_brackets_struct {
    /* ... */
};

void vertical_brackets_function(int some_parameter)
{
    if (egyptian_brackets_statement) {
        /* ... */
    }
}
```

## Comments
Code comments should be formatted like so:
```c
/* this is a code comment */
```

Multi-line comments:
```c
/*
 * Some very long description that
 * spans multiple lines.
 */
int foo(int bar) {
    /* ... */
}
```

## References
- https://www.kernel.org/doc/html/v4.10/process/coding-style.html
- https://developer.gnome.org/programming-guidelines/stable/c-coding-style.html.en
- https://www.gnu.org/prep/standards/html_node/Writing-C.html