# Lua Style Guidelines
The conventions detailed here are as close as possible to the official recommendations. As always, consistency within a project or organization is more important than rigid adherence to these conventions.

## Classes
Use `PascalCase` (metatables are used to simulate classes):
```lua
SomeClass = {}
SomeClass.__index = SomeClass

function SomeClass:new(some_field)
   local some_class = {}
   setmetatable(some_class, SomeClass)
   some_class.some_field = some_field
   return some_class
end
```

## Functions
Use `snake_case` for function name and `snake_case` for parameters:
```lua
function some_function(some_parameter)
    -- ...
end
```

## Variables
Use `snake_case`:
```lua
some_variable = 1
some_other_variable = some_method()
```

## Constants
Use `CONSTANT_CASE` (this is a convention as lua does not have constants):
```lua
SOME_CONSTANT = 1
```

## Abbreviations
Use `snake_case`:
- `io_reader`
- `html_button`
- `item_id`

## Comments
Code comments should be formatted like so:
```lua
-- this is a code comment
```

Documentation comments should use the LuaDoc format:
```lua
--- Description of the method that fits in one line.
-- Add a more elaborate description here that can span multiple lines.
-- @param bar Description of parameter.
-- @return Description of return value.
function foo(bar)
    -- ...
end
```

## References
- http://lua-users.org/wiki/LuaStyleGuide
- https://codingart.readthedocs.io/en/latest/lua/NamingConventions.html
- https://github.com/luarocks/lua-style-guide