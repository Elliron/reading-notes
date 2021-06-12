# 401 Class-03 FileO and Exceptions

## Reading and Writing Files in Python

- files are a set of bytes used to store data

- bytes are translated into binary

- Files contain three main parts
  - Header - metadata contents of file
  - Data - contents of file written by creator/editor
  - EOF - End of File, special char indicated end of file

- File Paths
  - Folder Path - file folder location
  - File name - name of file
  - iExtension - end of file path pre-pended with period.  indicates file type

- Line endings - new line, around since morse code
- Character Encoding - translation from bye data to human readable, ASCII or UNICODE
- Opening and Closing a file

  ```
  file = open('file_name.txt')
  ```

  ```
  reader = open('file_name.txt')
  try:
  finally:
    reader:close
    ```

    ```
    with open('file_name.txt') as reader
    ```

    - mode

    ```
    with python('file_name.txt', 'r') as reader:
    ```

- Three different file objects
  - Text files
  - Buffered binary files
  - Raw binary files

- Reading and Writing opened files
  - `.read(size=-1)`
  - `.readline(size=-1)`
  - `.readlines()`

- Iterate over each line

```
>>> with open('dog_breeds.txt', 'r') as reader:
>>>     # Read and print the entire file line by line
>>>     line = reader.readline()
>>>     while line != '':  # The EOF char is an empty string
>>>         print(line, end='')
>>>         line = reader.readline(
```

- `.write(string)`
- `.writelines(seq)`

```
with open('dog_breeds.txt', 'r') as reader:
    # Note: readlines doesn't trim the line endings
    dog_breeds = reader.readlines()

with open('dog_breeds_reversed.txt', 'w') as writer:
    # Alternatively you could use
    # writer.writelines(reversed(dog_breeds))

    # Write the dog breeds to the file in reversed order
    for breed in reversed(dog_breeds):
        writer.write(breed)
```

- byte strings - add b character to mode

## Python Exceptions
- Syntax errors - parser detects incorrect statement
- Exception errors - syntactically correct Python code results in error
  - raise - used to throw an exception if condition occurs
- AssertionError Exception - assert that a certain condition is met
- try and except - catch and handle exception
- Else - execute a certain block of code in absence of exceptions
- Finally - will always run


[Home](../README.md)
