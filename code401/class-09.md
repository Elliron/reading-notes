# Class 04

## Dunder Methods
- Special/Magic Methods - set of predefined methods to enrich classes.  Use Dunders
- Emulate the behavior of built-in types

```
class NoLenSupport:
    pass

>>> obj = NoLenSupport()
>>> len(obj)
TypeError: "object of type 'NoLenSupport' has no len()"
```

```
class LenSupport:
    def __len__(self):
        return 42

>>> obj = LenSupport()
>>> len(obj)
42
```

### Dunder Methods List

- ` __init__`
- `__repr__` 
- `__str__`
- `__len__` - 
- `__getitem__` -
- `__reversed__` - 
- `__eq__`
- `__lt__`
- `__add__`
- `__call__`
- `__enter__`
- `__exit__`


## Probability
- Odds of something happening
    - What could occur
    - Flip a coin 10 times and count how many times you get heads/tails.
    - May have an abnormally high count of heads or tails
    - The more times you run the test the closer you get to the true odds
- Three Sigma Rule - expression of how many observations fall within a certain distance of mean
- Z-score - "Given a data point, how many standard deviations is it away from the mean"

[Home](../README.md)
