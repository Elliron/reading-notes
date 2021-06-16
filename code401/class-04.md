# Class 04 Topic

## Classes and Objects

- Objects - encapsulation of variables and functions to make a single thing. Get variables and functions from classes.  Classes are a template to create objects.

## Thinking Recursively
- Iteration - counting from start to finish
- Recursion - Splits the work in half(functions calls itself)
- stack frame - each recursion call adds one to the call stack until it reaches the base case.

- Maintaining State - must do one of these
  - Thread through each recursive call
  - keep state in global scope

- Recursive Data Structure - defines in terms of smaller version of self

## Pytest Fixtures and Coverage

- Fixtures - objects available to all tests
  - `pytest.fixture` 

  ```
  def reverse_lines(f):
    return [one_line.rstrip()[::-1]+ '\n'
      for one_line in f]
  ```

  ```
  @pytest.fixture(scope='module')
  def simple_file():
   return StringIO('\n'.join(['abc', 'def', 'ghi', 'jkl']))
  ```

  - Coverage - pytest-cov on PyPI to download, invoke `--cov`



[Home](../README.md)