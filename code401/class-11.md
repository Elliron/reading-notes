# Numpy

Numpy - Python data analysis package

List of lists for csv data

``` python
import csv
with open('winequality-red.csv', 'r') as f:
    wines = list(csv.reader(f, delimiter=';'))

print(wines[:3])
```

2 - Dimensional Arrays

``` python
import csv
with open("winequality-red.csv", 'r') as f:
    wines = list(csv.reader(f, delimiter=";"))
import numpy as np
wines = np.array(wines[1:], dtype=np.float)
```

Read File

``` python
wines = np.genfromtxt("winequality-red.csv", delimiter=";", skip_header=1)
```

Index numPy Arrays

``` python
wines[2,3]
```

Slicing

``` python
wines[0:3,3]
```

Assign Values to arrays

``` python
wines[1,5] = 10
```

1-Dimensional arrays

``` python
third_wine = wines[3,:]
```

N-Dimensional arrays

``` python
[500, 505, 490, 810, 450, 678, 234, 897, 430, 560, 1023, 640]

year_one = [
    [500,505,490],
    [810,450,678],
    [234,897,430],
    [560,1023,640]
]

earnings = [
    [
        [500,505,490],
        [810,450,678],
        [234,897,430],
        [560,1023,640]
    ],
    [
        [600,605,490],
        [345,900,1000],
        [780,730,710],
        [670,540,324]
    ]

    earnings = np.array(earnings)
    earnings[0,0,0]
```

Data Types

``` python
wines.dtype
```

Converting Data Types

``` python
wines.astype(int)
```


[Home](../README.md)
