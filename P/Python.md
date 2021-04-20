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

## How to Assert

```
assert x == "goodbye", "x should be 'hello'"
```

Source

* Python assert Keyword
  * https://www.w3schools.com/python/ref_keyword_assert.asp

## To to add Keys and Values to a Dictionary

You create a new key/value pair on a dictionary by assigning a value to that key

```
d = {'key': 'value'}
print(d)  # {'key': 'value'}

d['mynewkey'] = 'mynewvalue'

print(d)  # {'key': 'value', 'mynewkey': 'mynewvalue'}
```

If the key doesn't exist, it's added and points to that value. If it exists, the current value it points to is overwritten.

Source

* How can I add new keys to a dictionary?
  * https://stackoverflow.com/questions/1024847/how-can-i-add-new-keys-to-a-dictionary

## How to Clear a String Without Create a New Object

?

Source

* Python String translate() Method
  * https://www.w3schools.com/python/ref_string_translate.asp
* Built-in Types
  * https://docs.python.org/3/library/stdtypes.html#string-methods

## How to Open a File

```
reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()
```

```
with open('dog_breeds.txt') as reader:
    # Further file processing goes here
```

Source

* Reading and Writing Files in Python (Guide)
  * https://realpython.com/read-write-files-python/

## How to Check If a File Exists

```
import os.path
path.exists("guru99.txt")
```

Source

* Python Check If File or Directory Exists
  * https://www.guru99.com/python-check-if-file-exists.html

## How to Compare Strings

Use == to compare by value.

Source

* Comparing Strings using Python
  * https://stackabuse.com/comparing-strings-using-python/

## How to Create a Matrix

```
>>> numpy.zeros((2, 1))
array([[ 0.],
       [ 0.]])
```

Source

* numpy.zeros
  * https://numpy.org/doc/stable/reference/generated/numpy.zeros.html

## How to List Files in a Directory

Source

```
from os import listdir
os.list()
```

* How do I list all files of a directory?
  * https://stackoverflow.com/questions/3207219/how-do-i-list-all-files-of-a-directory

## How to Remove a File

```
import os
os.remove("demofile.txt")
```

Source

* Python Delete File
  * https://www.w3schools.com/python/python_file_remove.asp

## How to Trim String

```
s = s.trim()
```

Source

* Python Trim String
  * https://www.journaldev.com/23625/python-trim-string-rstrip-lstrip-strip

## How to Check if a Character in a String is a Letter

```
c = "a"
c.isalpha()

```

Source

* How can I check if character in a string is a letter? (Python)
  * https://stackoverflow.com/questions/15558392/how-can-i-check-if-character-in-a-string-is-a-letter-python

## How to Check if a Key is in a Dictionary

You can use dict.get()

```
value = d.get(key)
```

which will return None if key is not in d. You can also provide a different default value that will be returned instead of None:

```
value = d.get(key, "empty")
```

Source

* Return None if Dictionary key is not available
  * https://stackoverflow.com/questions/6130768/return-none-if-dictionary-key-is-not-available