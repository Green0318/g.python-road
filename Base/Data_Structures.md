# Python data structures

``` 
In Python we have:
1.Integer(int)
2. Float
3.String(str)
4.List
5.Tuple
6.Dict
7.Set
8.Boolean Type
```

| Mutable     |  Immutable   |
|-------------|--------------|
 | List        | Int          |
 | Dict        | Float        |
| Set         | Str          |
|             | Tuple        |
|             | Boolean Type |








## Integers
An integer is a whole number with no decimal places. For example, 1 is an integer, but 1.0 isn’t.
The name for the integer data type is int, which you can see with type():
```python
x = 10
print(type(x))
# <class 'int'>
```
## Float
A floating-point number, or float for short, is a number with a decimal place.
1.0 is a floating-point number, as is -2.75. 
The name of the floating-point data type is float:
```python
x = 12.5
print(type(x))
# <class 'float'>
```
### Arithmetic Operators and Expressions numbers:
#### Addition:
```python
print(1+2)          # 3
print(1.0 + 2)      # 3.0

```
#### Subtraction:
```python
print(10 - 5)       # 5 
print(12.0 - 3)     # 9.
print(10 - 15)      # -5
```
#### Multiplication:
```python
print(3 * 6)        # 18
print(3.5 * 2)      #7.0
```
#### Division:
```python
print(20 / 5)       # 4
print(7 / 2)        # 3.5
```
#### Integer Division:
```python
print(10 // 3)      # 3
print(15 // 2)      # 7
print(7.5 // 3)     # 2.0
```
#### Exponents:
```python
print(2 ** 3)       # 8
print(4 ** 3 )      # 64
print(9 ** 0.5)     # 3.0
```
#### The Modulus Operator:
```python
print(5 % 2)        # 1
print(20 % 7)       # 6
```
## Strings

Besides numbers, Python can also manipulate strings, which can be expressed in several ways.
They can be enclosed in **single quotes** ('...') or **double quotes** ("...")
with the same result, \ can be used to escape quotes:
```python
print('Hi world')       # Hi world
print("Hi world")       # Hi world
print(type("Hi world"))      # <class 'str'>
```
#### Accessing characters in Python String:
Like many other popular programming languages, strings in Python are arrays of bytes
representing unicode characters. However, Python does not have a character data type,
a single character is simply a string with a length of 1.
Square brackets can be used to access elements of the string.
```python
s  = "Hello Python"
print(s[0])     # H
print(s[4])     # o
print(s[-1])    # n 
print(s[:5])    # Hello
print(s[6:])    # Python
print(s[::-1])  # nohtyP olleH
```
##### String length:
To get the length of a string, use the `len()` function.
```python
a = "Hello world"
print(len(a))       # 11
```
##### String Concatenation:
Strings, like numbers, can be added. 
The operation of adding strings is called concatenation or concatenation.
```python
s_1 = "Python is "
s_2 = "high-level "
s_3 = "programming language"
print(s_1 + s_2 + s_3 + "!!!")   # Python is high-level programming language!!!
```
In Python, you can also multiply a string by a number.
```python
s = "Hi"
print(s * 5)        # HiHiHiHiHi
```
## Strings methods
The most popular string methods
```python
# capitalize()    Converts the first character to upper case
test_0 = 'hello WoRLd'
test_1 = "HI EHOR"
print(test_0.capitalize())      # Hello world
print(test_1.capitalize())      # Hi ehor
# count()    Returns the number of times a specified value occurs in a string
print(test_0.count("o"))        # 2
print(test_1.count("h"))        # 0
# endswith()    Returns true if the string ends with the specified value
print("I am Vlad".endswith("d"))        # True
print(test_1.endswith("r"))             # False       
# find()    Searches the string  and returns the position of where it was found
print("Oh,shit".find("h"))      # 1
print("Im sorry".find("y"))     # 7
# isalnum()    Returns True if all characters in the string are alphanumeric
s = "13bruh3801"
print(s.isalnum())      # True
print("!@#$#%$#*".isalnum())        # False
# isalpha()    Returns True if all characters in the string are in the alphabet
print("Yes".isalpha())          # True
print("Yes123".isalpha())       # False
# isdigit()    Returns True if all characters in the string are digits
print("$1290".isdigit())        # False
print("106".isdigit())          # True
# islower()    Returns True if all characters in the string are lower case
print("hello world".islower())      # True
print("Hello World".islower())      # False
# isupper()    Returns True if all characters in the string are upper case
print("HELLO EVERYBODY".isupper())      # True
print("FDSNSLAVESJKs".isupper())        # False
# join()    Converts the elements of an iterable into a string
List = ["Three","Hundred","Bucks"]
print("$".join(List))           # Three$Hundred$Bucks
print("0".join("1"*8))          # 101010101010101
# lower()    Converts a string into lower case
print("VLAD".lower())       # vlad
print(test_0.lower())       # hello world
# upper()    Converts a string into upper case
print("just do it".upper())         # JUST DO IT
print("yes sir".upper())            # YES SIR
# lstrip()    Returns a left trim version of the string
print("    Lets go".lstrip())         # Lets go
print("    danger!".lstrip())        # danger!
# replace()    Returns a string where a  value is replaced with a specified value 
breakfast =  "My breakfast is  apple"
print(breakfast.replace("apple","burger"))      # My breakfast is  burger
print(breakfast.replace("My","Your"))           # Your breakfast is  apple
# rstrip()    Returns a right trim version of the string
print("I like it    ".rstrip())         # I like it
print('Python   '.rstrip())             # Python
# split()    Splits the string at the specified separator, and returns a list
print("Python,Java,C,Assembler".split(","))  # ['Python', 'Java', 'C', 'Assembler']
print("1!2!3!4!5!".split("!"))          # ['1', '2', '3', '4', '5', '']
# startswith()	Returns true if the string starts with the specified value
print("I like Python".startswith("I"))          # True  
print("I like Python".startswith("You"))        # False
# strip()    Returns a trimmed version of the string
print("    !King James!    ".strip())       # !King James!
print("    !MJ Goat!   ".strip())           # !MJ Goat!
# swapcase()    Swaps cases, lower case becomes upper case and vice versa
print("HI python".swapcase())           # hi PYTHON
print("wHO aRE yOU?".swapcase())        # Who Are You?
# title()    Converts the first character of each word to upper case
print("i want pizza".title())           # I Want Pizza
print("apple banana cherry".title())    # Apple Banana Cherry  
```
## List
Lists are used to store multiple items in a single variable.
Lists are one of 4 built-in data types in Python used to store collections of data,
lists are created using square brackets:
```python
the_list = ["apple", "banana", "orange", "cherry"]
print(the_list)     # ['apple', 'banana', 'orange', 'cherry']
```
#### List items are ordered, changeable, and allow duplicate values:
```python
the_list = ["apple", "banana", "apple" ,  "orange", "cherry"]
print(the_list[0])   # apple
the_list[-1] = "dragon fruit"
print(the_list)      # ['apple', 'banana', 'apple', 'orange', 'dragon fruit']
```
#### Basic list function:
```python
num_list = [12,21,78]
print(len(num_list))    # 3
print(max(num_list))    # 78
print(min(num_list))    # 12
print(sum(num_list))    # 111
print(num_list * 2)     # [12, 21, 78, 12, 21, 78]
```
#### Print a list of elements:
```python
#1
numbers = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
for num in numbers:
    print(num)
#2
numbers = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
print(*numbers)
```
#### List comprehension
```python
numbers = [i for i in range(10)]
squares = [i ** 2 for i in range(10)]
lines = [input() for _ in range(int(input()))]
```
### List Methods
```python
#append()    Adds an element at the end of the list
list_0 = [1,2,3,4]
list_0.append(12)
print(list)     # [1, 2, 3, 4, 12] 
list_0.append([10,78])
print(list)     # [1, 2, 3, 4, 12, [10, 78]]
#clear()    Removes all the elements from the list
list_1  = [65,76,87,98,12]
list_1.clear()
print(list)         # <class 'list'>
#copy()    Returns a copy of the list
list1 = [1,2,3,4,5,"Yes"]
list2 = list1.copy()
print(list2)        # [1, 2, 3, 4, 5, 'Yes']      
print(list2 == list1)       # True
#count()    Returns the number of elements with the specified value
test_count = [1,1,8,"bio",4,1]
print(test_count.count(1))      # 3
#extend()    Add the elements of a list (or any iterable), to the end of the current list
test_count.extend([45,1,78])    
print(test_count)           # [1, 1, 8, 'bio', 4, 1, 45, 1, 78]
test_count.extend("Hello")
print(test_count)           # [1, 1, 8, 'bio', 4, 1, 45, 1, 78, 'H', 'e', 'l', 'l', 'o']
#index()    Returns the index of the first element with the specified value
print([23,65,43,2].index(2))        # 3
#insert()    Adds an element at the specified position
test = ["pizza","burger","coke"]
test.insert(1,"sprite")
print(test)         #['pizza', 'sprite', 'burger', 'coke']
#pop()    Removes the element at the specified position
test.pop(2)
print(test)     # ['pizza', 'sprite', 'coke']
test.pop()
print(test)     # ['pizza', 'sprite']
#remove()    Removes the first item with the specified value
l = [16,98,56,4]
l.remove(98)
print(l)        # [16, 56, 4]
#reverse()    Reverses the order of the list
l.reverse()
print(l)        # [4, 56, 16]
#sort()    Sorts the list
l.sort()
print(l)        # [4, 16, 56]
```
## Tuple
Tuples are used to store multiple items in a single variable.
A tuple is a collection which is ordered and *unchangeable*.
Tuples are written with round brackets
```python
the_tuple = (21,90,"programming",True)
print(the_tuple)        # (21, 90, 'programming', True)
```
#### Tuple items are ordered, allow duplicate values but unchangeable:
```python
test_tuple  = (21,90,"programming",True,["apple","fruit"])
print(test_tuple[2])        # programming
print(test_tuple[-1][0])        # apple
test_tuple[2] = 18      #'tuple' object does not support item assignment
test_tuple[-1][1] = "vegetable"
print(test_tuple)       #(21, 90, 'programming', True, ['apple', 'vegetable'])
```
#### In tuple basic functions, like in list
```python
num_tuple = [15,24,78]
print(len(num_tuple))    # 3
print(max(num_tuple))    # 78
print(min(num_tuple))    # 15
print(sum(num_tuple))    # 117
print(num_tuple * 2)     # [12, 21, 78, 12, 21, 78]
```
### Tuple methods
```python
#count()	Returns the number of times a specified value occurs in a tuple
thistuple = (1, 3, 7, 8, 7, 5, 4, 6, 8, 5)
x = thistuple.count(5)
print(x)        # 2        
#index()	Searches the tuple for a specified value and returns the position of where it was found
test_tuple = (1,3,6,8,1,2)
print(test_tuple.index(3))      # 1
```
## Dict
Dictionaries are used to store data values in key:value pairs.
A dictionary is a collection which is ordered*, changeable and do not allow duplicates.
Dictionaries are written with curly brackets, and have keys and values:
```python
test_dict = {
    "name" : "Aleks",
    "year" : 1980,
    "height" : 6.5    
}
print(test_dict)        # {'name': 'Aleks', 'year': 1980, 'height': 6.5}
```
Dictionary items:
```python
test_dict = {
    "name" : "Aleks",
    "year" : 1980,
    "height" : 6.5    
}
print(test_dict["height"])      # 6.5
```
Duplicates on dictionary:
```python
test_dict = {
    "name" : "Aleks",
    "year" : 1980,
    "height" : 6.5,
    "year" : 1995
}
print(test_dict["year"])        # 1995
```
The values in dictionary items can be of any data type:
```python
test_dict = {
    "name" : "Anton",
    "age" : 23,
    "hobbies" : False,
    "list_of_pets" : ["dog","cat","hamster"]
}
```
### Dict methods
```python
#clear()  Remove all the elements from the dictionary
dict = {
    "one" : 1,
    "two " : 2,
    "three" : 3
}
print(dict.clear())     # None
#copy()  Returns a copy of the dictionary
dict_0 = {
    "one" : 1,
    "two " : 2,
    "three" : 3
}
dict1 = dict_0.copy()
print(dict1)        # {'one': 1, 'two ': 2, 'three': 3}
#get()  Returns the value of specified key
test_dict = {
    "Math" : 87,
    "English" : 68,
    "Chemistry" : 55,
    "Physics" : 91
}
print(test_dict.get("Math"))        # 87
#items()  Returns a list containing a tuple for each key value pair
print(test_dict.items())            # dict_items([('Math', 87), ('English', 68), ('Chemistry', 55), ('Physics', 91)])
#keys()  Returns a list containing dictionary’s keys
print(test_dict.keys())         # dict_keys(['Math', 'English', 'Chemistry', 'Physics'])
#pop()  Remove the element with specified key
test_dict.pop("Chemistry")
print(test_dict)            #{'Math': 87, 'English': 68, 'Physics': 91}
#popitem()  Removes the last inserted key-value pair
item = test_dict.popitem()
print(test_dict)        # {'Math': 87, 'English': 68}
print(item)             #('Physics', 91)
#update()  Updates dictionary with specified key-value pairs
test_dict.update({item})
print(test_dict)        # {'Math': 87, 'English': 68, 'Physics': 91}
#values()  Returns a list of all the values of dictionary
print(test_dict.values())       # dict_values([87, 68, 91])

```
## Set
Sets are used to store multiple items in a single variable.
Set is one of 4 built-in data types in Python used to store collections of data,
A set is a collection which is unordered, unchangeable*, and unindexed.
```python
test_set = {"apple",243,"banana",True}
print(test_set)     # {'apple', True, 'banana', 243}
# Sets are unordered, so you cannot be sure in which order the items will appear
```
Set items are unordered, unchangeable, and do not allow duplicate values.
```python
test_set = {"name","height","weight","name"}
print(test_set)     # {'name', 'height', 'weight'}
```
### Set methods
```python
#add()	Adds a given element to a set
#clear()	Removes all elements from the set
#copy()	Returns a shallow copy of the set
#difference()	Returns a set that is the difference between two sets
#difference_update()	Updates the existing caller set with the difference between two sets
#discard()	Removes the element from the set
#frozenset()	Return an immutable frozenset object
#intersection()	Returns a set that has the intersection of all sets
#intersection_update()	Updates the existing caller set with the intersection of sets
#isdisjoint()	Checks whether the sets are disjoint or not
#issubset()	Returns True if all elements of a set A are present in another set B
#issuperset()	Returns True if all elements of a set A occupies set B
#pop()	Returns and removes a random element from the set
#remove()	Removes the element from the set
#union()	Returns a set that has the union of all sets
#update()	Adds elements to the set
```
## Boolean Type
Python boolean type is one of the built-in data types provided by Python, which represents one of the two values i.e. 
True or False. Generally, it is used to represent the truth values of the expressions. For example, 1==1 is True whereas 2<1 is False.
```python
a = True
b = False
print(type(a))      # <class 'bool'> 
print(type(b))      # <class 'bool'>
```
#### Method `bool()` 
```python
x = 5
y = 10
print(bool(x > y))      # False
a = 10 -5
b = 5
print(bool(a==b))       # True
```
### Boolean operators
| A	    | B	     | A or B |
|-------|--------|--------|
| True  | 	True  | 	True  |
| True  | 	False | 	True  |
| False | 	True  | 	True  |
| False | 	False | 	False |

| A	    | B	     | A and B |
|-------|--------|---------|
| True  | 	True  | 	True   |
| True  | 	False | 	False  |
| False | 	True  | 	False  |
| False | 	False | 	False  |

| A	    | Not A  |
|-------|--------|
| True  | 	False |
| False | 	True  |

