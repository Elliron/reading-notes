# Python Scope

- Scope - how variables and names are looked up in code
    - visibility of variable within code
    - LEGB - Local, Enclosing, Global, Built in
    - defines area of program where you can unambiguously access the name of a variable, function, object, etc.
    - implemented as dictionaries called namespace
    - In Scope = have access too, Out of Scope = no access

- Global - available to all code
    - assign a name outside of all functions
- Local - only available to code within a local scope
    - assign a name in a function
    - created at function call not definition
- Enclosing - special scope for nested functions
    - inner scope would be local, outer scope would be enclosing.
- Built In - created/loaded when script is ran or open interactive session
    - contains - keywords, functions, exceptions, and other built in attributes
    - `__builtins__` - names in builtins are always loaded in global scope with this name
- available anywhere in code, provided by python
- `__main__` - turns main script into a module that holds the main programs execution 
    - global scope


- Namespace - dictionaries that implement scope 

```
import sys
sys.__dict__.keys()
```

  - names at top level module are stored here
  - python will return the first variable or function name that matches your search

- Global Statement - define a list of names to be treated as global

```
counter = 0  # A global name
>>> def update_counter():
...     global counter  # Declare counter as global
...     counter = counter + 1  # Successfully update the counter
...
>>> update_counter()
>>> counter
1
>>> update_counter()
>>> counter
2
>>> update_counter()
>>> counter
3
```
- nonlocal statement - accessed from inner functions but not assigned or updated

```
nonlocal my_var  # Try to use nonlocal in the global scope
  File "<stdin>", line 1
SyntaxError: nonlocal declaration not allowed at module level
>>> def func():
...     nonlocal var  # Try to use nonlocal in a local scope
...     print(var)
...
  File "<stdin>", line 2
SyntaxError: no binding for nonlocal 'var' found
```

- import - use import to bring seperate modules to your __main__ module
- comprehension - compact way to process all or part of elements in collection or sequence
    - can be brackets [], or culry braces {} containing an expression, followed by one or more for clauses and zero or one if statements per for clause
- exceptions - variable holds reference to exception raised by try statement
- class and instance - defining a class creates a new local scope.
    - names assigned at top are local
    - created at execution
- `globals()` - returns reference to current global scope or namespace dict
- `locals()` - updates and returns dict that holds copy of current state of local scope or namespace
- `vars()` - builtin function that returns .__dict__ attribute of module, class, instance or any other object with dict attribute
- `dir()` - can use without arguments to get list of names in current scope, with argument function will try to return a list of valid attributes for object


[Home](../README.md)