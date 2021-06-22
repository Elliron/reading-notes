# Class 06

## How to Random Module
- Provides access to functions that support many operations
- Generates random numbers
- Randint - accepts two parameters(lowest_number, highest_number)

```
import random
print random.randint(0, 5)
```
- can multiple for larger numbers

- Choice - generate a random value from a sequence
```
random.choice( ['First Choice', 'Second Choice', 'Third Choice'])
```

- Shuffle - shuffles elements in the list in place so they are in a random order

```
from random import shuffle
x = [[element_in_list]] for element_in_list in range(10)]
shuffle(x)
```

- randrange- Generates a randomly selected element from range(start, stop, step)
```
import random
for i in range(3):
    print random.randrange(0, 101, 5)
```
- chooses two outcomes
```
import random
import itertools

outcomes = { 'heads':0,
             'tails':0,
             }
sides = outcomes.keys()

for i in range(10000):
    outcomes[ random.choice(sides) ] += 1

print 'Heads:', outcomes['heads']
print 'Tails:', outcomes['tails']
```

## What is Risk Analysis

- Risk - probability of unwanted incident
- process of identifying risks in apps or software that you built and prioritizing them to test.
- find the risk areas before they become a problem, the earlier the better.
- Unavoidable risks
  - time allocated for testing
  - defect leakage due to complexity of size of app
  - Urgency to deliver
  - Incomplete requirements

- Three levels of risk
  - High
  - Medium
  - Low

- Risk ID
    - Business
    - Testing
    - Premature Release
    - Software

- Risk Assessment
    - Effect
    - Cause
    - Likeliehood

- Three steps to perform Risk Analysis
    - Searching the risk
    - Analyzing the impace of each individual risk
    - Measure for risk indentified

## Big O Notation
- Algorithm Efficiency
- Transfering Data over the internet changes based on the amount of data being transferred.
- O(1) constant time with respect to the sizes of input, doesnt take longer with more input
- O(N) Scales linearaly with the amount of input, twice as much data takes twice as much time.
    - N is the size of the List

- Different steps in algorithm, add them together
- Drop constants
- Different inputs use different variables
- Drop non-dominant terms

[Home](../README.md)
