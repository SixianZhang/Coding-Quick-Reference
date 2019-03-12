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

## Character

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

## **Array**

## **List**

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

## **while**

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

## **switch**

## **try...catch**




# Method and function
<a name= "#method-and-function"></a>

## **Example Code**


# Class
<a name= "#class"></a>

## **Example Code**

## **Field variable**

## **Field methods**

## **Override methods**

## **Inheritance**

## **Others**

# Package
<a name = #package></a>

# Input and output
<a name= "#input-and-output"></a>

# Error and exception
<a name= "#error-and-exception"></a>


# Coding style
<a name= "#coding-style"></a>


# Libraries
<a name= "#libraries"></a>

# Arithematic calculation
<a name= "#arithematic-calculation"></a>