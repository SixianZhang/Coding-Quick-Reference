# Content Table 
* [Intro](#intro)
* [Conmand Window](#command-window)
* [Data](#data)
* [Control flow](#control-flow)
* [Method and function](#method-and-function)
* [Class](#class)
* [Package](#package)
* [Input and output](#input-and-output)
* [Error and Exception](#error-and-exception)
* [Coding style](#coding-style)
* [Libraries](#libraries)
* [Arithematic calculation](#arithematic-calculation)

# Intro 
<a name= "#intro"></a>
This is a quick reference for Python language with only examples and some comments.

# Command Window
<a name = "command-window"></a>

# Data 
<a name= "#data"></a>

## **Example Code**

## **Primitive Data**
### int

### float

### double

### operators

### convertion

## Boolean

---
## Character
```Python
a = 'a'
ord(a) # ascii code of 'a'

b = 105
chr(b) # character of ascii code for b
```
**Note:**
1. String with one element is a character.
2. ord and chr methods only work for character.

---

## String
```python
a = 'Hello'
print(a)
print(a[1]) # will print out e

# Following code will not work since string is immutable. You can't modify a string by elements. 
a[1] = 'a'
a.remove('a')

b = 'hello' 
a < b # True, character by character comparision

len(a) # 5

a[-2] # l, count backward, -1 is the last one
a[-2:] # lo, last two characters
a[2:100] # show the string till the end, this won't work if you only access one element

a = a + ' people'

'Hello ' 'people' # 'Hello people', only viable when no variable exist

>>> a[-100:100] # This won't raise error.
```
**Note:** 
1. The most tricky part of the string is that if you access str[a:b], it will actually give you element from a to b - 1. This works the same for **range** function.
1. String is not an **array**. Although it works like an array. Python does not have **array**.
1. ToString function in python is **\_\_str\_\_**. 
1. The index can't exceed the range of the string (0 to len(str)) when you access one element, but it would be fine if you are accessing a slide of the string.
---

## **Array**
**Note:**
1. Seems Python does not have a built-in array. It uses array module to achieve array.
---
 
## **List**
```python
# Create an empty list
a = list()

# List is a object
a = [1,2,3,4]
b = a
a[1] = 100
# a and b will both change to [1,100,3,4] since list is an object.

# Copy a list
c = list(a) # This will create a new list object which has the same content as a
c.append(200)
# This change won't affect a and b, since they are different list object.

```
**Note:**
1. **LIST IS A NON-PRIMITIVE DATA TYPE!!!** List is a object, so the change to the reference pointing to a list will also affect other references pointing to the same list.
2. Although **string** works like a list(or array), but a string is **immutable**, while list is **mutable**. 
---

## **Tuple**
```python
    t = 12345, 54321, 'hello'
    t[0] # 12345
    t   # (12345, 54321, 'hello')

    # Nested tuple
    u = t, (1,2,3,4,5)
    u   # ((12345, 54321, 'hello'),(1,2,3,4,5)) 

    # Tuple is immutable
    t[0] = 8888 # This is invalid

    v = ([1,2,3,4],[4,3,2,1])
```


## **Dictionary**

## **Set**

## **Enumerat**

## **Structure**


# Control flow
<a name= "#control-flow"></a>

## **if...else**
```python
if x < 0:
     x = 0
     print('Negative changed to zero')
 elif x == 0:
     print('Zero')
 elif x == 1:
     print('Single')
 else:
     print('More')
```
**Note:** 
* **if...elif...else** sequence can be used as a substitute of **switch case** statement. 
---
## **while**
---
## **for**
```python
for n in range(2, 10):
     for x in range(2, n):
         if n % x == 0:
             print(n, 'equals', x, '*', n//x)
             break
     else:
         # loop fell through without finding a factor
         print(n, 'is a prime number')
```
**Note:**
* **range()** function can be replaced by a iterable item, such as a list.
* Use **pass** if there is no statement in your loop structure, same to **if** statement.
---

## **switch**

## **try...catch**




# Method and function
<a name= "#method-and-function"></a>

## **Example Code**


**Note:**
1. Python pass primitive data by value, non-primitive data by reference.

# Class
<a name= "#class"></a>

## **Example Code**

## **Field variable**

## **Field methods**

## **Override methods**

### \_\_eq\_\_
**Note:**
1. This method will override the "==" operation
2. When calling **a==b**, it will call the \_\_eq\_\_ method from a, instead of from both of them.


## **Inheritance**

## **Others**

# Package
<a name = #package></a>

# Input and output
<a name= "#input-and-output"></a>

# Error and exception
<a name= "#error-and-exception"></a>

# Test
<a name = '#test'></a>
```python
import unittest
import ClassToBeTest

class ClassTest(unitest.TestCase):
    def setup(self):
    # This method run before the tests
        pass

    def teardown(self):
    # This method run between the tests
        pass
    
    # Below are the test methods
    def test1(self):
        self.assertEqual(a,b) # assert equals.
    
    def test2(self):

if __name__ = '__main__':
    unittest.main(verbosity = 2)
```
**Note:** 
1. Find more at https://docs.python.org/3/library/unittest.html#assert-methods
1. **Verbosity** argument control the information showed in the result.
1. The test will run in an alphabet order.




# Coding style
<a name= "#coding-style"></a>


# Libraries
<a name= "#libraries"></a>

# Arithematic calculation
<a name= "#arithematic-calculation"></a>
