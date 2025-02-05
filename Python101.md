```python
# Python Basics
```

## Whitespace Is Important


```python
listOfNumbers = [1, 2, 3, 4, 5, 6]

for number in listOfNumbers:
    print(number)
    if (number % 2 == 0):
        print("is even")
    else:
        print("is odd")
        
print ("All done.")
        
```

    1
    is odd
    2
    is even
    3
    is odd
    4
    is even
    5
    is odd
    6
    is even
    All done.
    

## Importing Modules


```python
import numpy as np

A = np.random.normal(25.0, 5.0, 10)
print (A)
```

    [26.21600415 24.76108062 25.29035418 19.82236898 30.9802717  22.09212022
     31.06977121 25.88557185 27.63390354 28.45243622]
    

## Lists


```python
x = [1, 2, 3, 4, 5, 6]
print(len(x))
```

    6
    


```python
x[:3]
```




    [1, 2, 3]




```python
x[3:]
```




    [4, 5, 6]




```python
x[-2:]
```




    [5, 6]




```python
x.extend([7,8])
x
```




    [1, 2, 3, 4, 5, 6, 7, 8]




```python
x.append(9)
x
```




    [1, 2, 3, 4, 5, 6, 7, 8, 9]




```python
y = [10, 11, 12]
listOfLists = [x, y]
listOfLists
```




    [[1, 2, 3, 4, 5, 6, 7, 8, 9], [10, 11, 12]]




```python
y[1]
```




    11




```python
z = [3, 2, 1]
z.sort()
z
```




    [1, 2, 3]




```python
z.sort(reverse=True)
z
```




    [3, 2, 1]



## Tuples


```python
#Tuples are just immutable lists. Use () instead of []
x = (1, 2, 3)
len(x)
```




    3




```python
y = (4, 5, 6)
y[2]
```




    6




```python
listOfTuples = [x, y]
listOfTuples
```




    [(1, 2, 3), (4, 5, 6)]




```python
(age, income) = "32,120000".split(',')
print(age)
print(income)
```

    32
    120000
    

## Dictionaries


```python
# Like a map or hash table in other languages
captains = {}
captains["Enterprise"] = "Kirk"
captains["Enterprise D"] = "Picard"
captains["Deep Space Nine"] = "Sisko"
captains["Voyager"] = "Janeway"

print(captains["Voyager"])
```

    Janeway
    


```python
print(captains.get("Enterprise"))
```

    Kirk
    


```python
print(captains.get("NX-01"))
```

    None
    


```python
for ship in captains:
    print(ship + ": " + captains[ship])
```

    Enterprise: Kirk
    Enterprise D: Picard
    Deep Space Nine: Sisko
    Voyager: Janeway
    

## Functions


```python
def SquareIt(x):
    return x * x

print(SquareIt(2))

```

    4
    


```python
#You can pass functions around as parameters
def DoSomething(f, x):
    return f(x)

print(DoSomething(SquareIt, 3))
```

    9
    

#Lambda functions let you inline simple functions
print(DoSomething(lambda x: x * x * x, 3))

## Boolean Expressions


```python
print(1 == 3)
```

    False
    


```python
print(True or False)
```

    True
    


```python
print(1 is 3)
```

    False
    


```python
if 1 is 3:
    print("How did that happen?")
elif 1 > 3:
    print("Yikes")
else:
    print("All is well with the world")
```

    All is well with the world
    

## Looping


```python
for x in range(10):
    print(x)
```

    0
    1
    2
    3
    4
    5
    6
    7
    8
    9
    


```python
for x in range(10):
    if (x is 1):
        continue
    if (x > 5):
        break
    print(x)
```

    0
    2
    3
    4
    5
    


```python
x = 0
while (x < 10):
    print(x)
    x += 1
```

    0
    1
    2
    3
    4
    5
    6
    7
    8
    9
    

## Activity

Write some code that creates a list of integers, loops through each element of the list, and only prints out even numbers!


```python

```
