# Python

## ...

```
{:.2f}.format(number)
```

Source

* How to specify the number of decimal places in Python
  * https://www.kite.com/python/answers/how-to-specify-the-number-of-decimal-places-in-python

## How to Calculate a Cross Product?

```
> x = [1, 2, 3]
> y = [4, 5, 6]
> np.cross(x, y)
array([-3,  6, -3])
```

Source

* numpy.cross
  * https://numpy.org/doc/stable/reference/generated/numpy.cross.html

## How to Normalise a Vector

```
an_array = np.random.rand(10)*10
norm = np.linalg.norm(an_array)
normal_array = an_array/norm
```

Source

* How to normalize an array in NumPy in Python
  * https://www.kite.com/python/answers/how-to-normalize-an-array-in-numpy-in-python

## How to Pass an Integer by Reference

* Integers are passed by value.
* Objects are passed by reference.
* Put integers in objects to pass by reference.

Source

* Passing an integer by reference in Python
  * https://stackoverflow.com/questions/15148496/passing-an-integer-by-reference-in-python

## split

Remember that Python passes by pointers and not refeence for objects.

If you want to split the original list, you can for example use pop() for the front and pop(-1) for the end.

Source

* Python List pop()
  * https://www.programiz.com/python-programming/methods/list/pop

## clear()

Available from Python 3.3 onward.

You can use del l[:].

Source

* Python3 AttributeError: 'list' object has no attribute 'clear'
  * https://stackoverflow.com/questions/32055768/python3-attributeerror-list-object-has-no-attribute-clear

## Type

```
type()
```

Source

* Get / determine the type of an object in Python: type(), isinstance()
  * https://note.nkmk.me/en/python-type-isinstance/

## Version

```
import sys
sys.version_info
```

Source

*
  * https://flaviocopes.com/python-check-version/#:~:text=You%20can%20check%20the%20version,running%20a%20program%2C%20at%20runtime.&text=Then%20check%20the%20content%20of,Python%20version%20as%20a%20tuple.