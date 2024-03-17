---
aliases:
  - Introduction to programming
Credits: 4
Done: true
tags:
  - CompSci/programming/Python
---
## Lecture 2:

- Command-line mode vs script-mode
- Arithmetic operators:
    - % modulus
    - ** exponential
    - // floor division
- Comparison, logical, identity, membership, bitwise operators:

## Lecture 4:

- Python function is part of the python script file, whereas methods are defined inside a class definition
- We can call a function directly if it’s in the same module or import a module and then call the function directly. To call a method, we need a class or an object of the class
- Python functions can access all the global variables, whereas Python class methods can access global variables, class attributes, and functions

```python
def exampleFunction(parameter1, parameter2 = "example string"): 
		#parameter2 default value if there is no argument
		print("")
```

![Screenshot 2022-10-19 at 15.55.46.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ca71c012-3ecb-480c-8724-033aa3ec8c81/Screenshot_2022-10-19_at_15.55.46.png)

## Lecture 5:

- Module is a smaller library, defined by someone
- Variable+value = an object
- The variable is redefined inside a function doesn’t change the value of the global variable

```
def f4() :
    print(s)
    s = "I'm Harry Potter's Friend"
    print(s)
s = "I'm Ali Baba's Friend"
f4()
print(s)
```

- The function f4 is called first without knowing what is s so error found
- The interpreter only read the functions and methods
- If global variable is defined within a function, the global will replace the local

```python
import math  
help <module> #see the library, press ENTER to see more
import math as m  #import a created instance
from math import *  #import all
from math import pow. #import only function pow
pow (2,3) # call directly, no need instance

naturalE = math.e #separate the variable
```

- Creating your own module:
    
    ```python
    a = 3
    def functionExample():
    	print()
    
    def greeting():
    	print()
    ```
    

## Lecture 7: String

- Sequences:
    - String
    - List
    - Tuples
- String & string manipulation:
    - String are immutable, all string methods returns another string
        
        ```python
        >>> exampleString = "Hello"
        >>> exampleString[0] = 'M' 
        # error 'str' object does not support item assignment
        >>> 'M' + exampleString[1:]
        'Mello' # overwritten the string
        ```
        

## Lecture 8:

```python
>>> len(string)
# length of the string

#string slicing
>>> exampleString[3]
# the character at third index, first index is 0
>>> exampleString[-1]
# the character at last index, -2 for second to last
print("Note: string slice doesnt include the last index ")
>>> exampleString[1:4]
# another string from 1 to 3, ignore 4
>>> exampleString[:]
# equivalent to exampleString[0:len(exampleString)]
>>> exampleString[::]
# same as x[0:len(exampleString):1]
>>> exampleString[1:4:2]
# another string from 1 to 2, skip by step of 2
>>> exampleString[3::-2]
# another string from 3rd to last strep of -2
>>> exampleString[::-1]
# reverse the string

#in
>>> if("test" in exampleString): #check for substring
>>> if(exampleString[::-1] in exapmString): #return True, as in 
>>> if("test" not in exampleString):

#is
>>> if(exampleString is "test"): #compare

#upper isupper
>>> exampleString.isupper()
# boolean
>>> x = examplestring.upper()
# upper case string

#index()
>>> exampleString.index("test") 
# the index of first letter that string test is in
>>> exampleString.index("test",0,10)
# the index only in range of from 0 to 10

#count()
>>> exampleString.count("test") 
# the count the frequency of the string "test" in the exampleString

#strip()
>>> exampleString.strip("a") 
# remove all letter 'a' from the beginning and end
>>> "Harry Potter".strip("H er") 
#remove H and er then = "arry Pott"

#split()
>>> exampleString.split(" ') 
#split by every in the middle space

#replace()
>>> exampleString.replace("yo", "hey") 
#change all "yo" to "hey"

#is
>>> exampleString.isnumeric() #check if its all digits
>>> exampleString.isalpha() #check if its characters
>>> exampleString.isalnum()
>>> exampleString.isdigit()
>>> exampleString.isdecimal()

>>> print("\\'")
'
>>> print("\\"")
"
>>> print("\\n")

>>> print("\\t")
|
>>> print""\\\\"")
/

#random
>>> import random
>>> random.choice(exampleString)
# return a random char in the string
>>> random.choice("yo")
# y or o
```

- Precondition: a condition that must always be true just before the execution of some section of codes or before an operation in a formal specification
    
    - Might or might not work as intended
    
    ```python
    >>> exampleString[:3] #means exampleString has to be string
    ```
    

![Screenshot 2022-10-26 at 16.08.03.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8be8f623-6d10-4d2b-a4a9-7cce218a219a/Screenshot_2022-10-26_at_16.08.03.png)

- Syntax error: indentation
    
- Runtime error: division, incompatible types, using undefined identifier, accessing non-existed elements
    
- Semantic error: output is meaningless
    
    - (“my age is cs”)
- Logical error: output is wrong, unintended
    
    - (“my age is 1”)
- Breakpoint: use the red dot mark on Pycharm, VScode
    
- Assertion and handling exceptions:
    
    - Assertions: to test the correctness of your code by checking if some specific conditions remain TRUE
        
        - If the assertion condition is false, then the assertion raises an exception and terminates the program's execution
        
        ```python
        my_age = int(input ("How old are you?")) 
        assert my_age > 0, f"Alo, are you sure you are {my age}?"
        """if true, skip
        if false, run the exception
        """
        ```
        
    - Exception handling:
        
        - A process of responding to the occurrence of exceptions – anomalous or exceptional conditions requiring special processing – during the execution of a program
            - try statements run first; if an error mentioned in one except’s arguments happened while running then except’s statements run, else the else statement run then the finally statements always run
        
        ```python
        try:
        		x = int(input("Type integer only, no text"))
        except(TypeError): #arguments of error type, more than one excepted
        		print("Only integer please, stupid?")
        else: #optional
        		print("very nice, thank you")
        finally: #optional
        ```
        

## Lecture 9:

- Conditionals: if-statements
    
    ```python
    if <condition(s)>:
    	<statements(s)>
    elif <condition(s)>:
    	<statement(s)>
    else:
    <nextStatement(s)>
    ```
    
- If -else vs nested if-else
    

## Lecture 10: Memory in Python

- Memory is for using data structure
- Memory management:
    - Efficiently allocating
    - Deallocating
    - Coordinating memory
- Memory allocation: allocation of a space (or a block) in the computer memory
- Garbage collector: automatically handles memory allocation and deallocation
- Private heap: contains all Python objects and data structure
- Garbage collection: process which the interpreter frees up the memory (when not in use) to make the available memory for ???

```python
import sys
v1 = 10
v2 = v1 
v3 = v2 
#3 objects point toward same memory address
address1 = sys.getrefcount(v1) #check the memory address of v1 variable
```

## Lecture 11&12: Objects , list & sequences

- List is one of built-in structures; together with tuples, dictionaries, and set
    - List are mutable, sequence types

![Screenshot 2022-11-07 at 15.57.38.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/bdc88c7f-8715-42c8-987e-ba750b492561/Screenshot_2022-11-07_at_15.57.38.png)

- Identical vs equivalent: is vs ==
    - is compare the pointer address
    - == compare the value
    - Every list is different object from the other list, equivalent but not identical
        - a=[1], b = [1] then (a ==b) = True
        - a = [1], b = a then they have same pointer address so (a is b) = True
        - except 2 empty list ( a=[], b=[] then (a is b) is True)

```python
>>> example_List = ["exampleString", 12, ...]
>>> empty = [] 
# store elements of different data types, separated by commas
>>> print(empty) 
[]

# slicing list and len works the same way as string

>>> a = [1,2,3,4]
>>> b = [9,10]

>>> a.append(5)
a = [1,2,3,4,5]
>>> a.remove(7)
ValueError # find the first element equal to 7 and delete it
>>> a.pop(4)
a = [1,2,3,4] #remove element at idex 4, if empty remove index -1

>>> a.extend(b) 
a = [1,2,3,4,9,10] # add each element one by one
>>> a.append(b) # add the objects as last element of the list, nested list
a = [1,2,3,4,9,10,[9,10]] # the last element is a list

>>> a.insert(1,5) #add in position 1, element 5
					# a = [1,5,2,3,4,9,10,[9,10]]
>>> a[1,3] = [0,0] # a = [1,0,0,3,4,9,10,[9,10]]

>>> a + b # list concatenation
>>> a + [0,0] # extends 2 more
>>> language = ["Java", "Python", "C++"]
>>> new_language = ["Pascal", "VB"]
>>> language[2:2] = new_language #insert a list and push the rest of elements back

>>> a = [1,1,2,3,4]
>>> a.count(1) 
2
>>> a.index(3) 
3
>>> a.index(5)
# ValueError: not in list

>>> a = list("hello") 
>>> a
["h", "e", "l", "l", "o"] # a list of 5 string elements of 1 letter each
>>> b = "I<3U"
>>> b.split("3")
["I", "3U"] # a list of elements separated by '3'
>>> "".join(a) 
hello # joins all the characters to have a string, 
>>> "*".join(a) 
h*e*l*l*o # join all the characters with '*' in the middle to form a string

>>> lettersList.sort() 
# method sort random letters within the list, as same as
>>> alphabet = sorted(lettersList) 
# function sort random letters and return another list
>>> alphabet = sorted(lettersList, reversed = True)
# sort then reverse

>>> a = ["a", "b", "c", "d"]
>>> a.reverse() 
["d", "c", "b", "a"] # method, change the self list to, as same as
>>> b = reversed(a) # a function 
#returns an iterator that accesses the given sequence in the reverse order

# 2-dimensional lists, nested list can be thought as 2d list
>>> my2dList = 
[
[1,2,3,4]
[5,6,7,8]
[9,10,11,12]
]

>>> my2dList[0,2] = 3 # row first then column

# enumerate(x)
x = ["a", "b", "c", "d"]
for i in enumerate(x):  # enumerate(x) returns [ (0, "a"), (1, "b"), (2, "c"),...]
												# like a dictionary

for i in enumerate(x,5):  # return dictionary but first element's index is 5
													# [ (5, "a"), (6, "b"), (7, "c"),...]

for i, item in enumerate(x,1): # so i is assigned as idex and item is elements
```

- Memory:
    - A list is a single object
    - Each object has the following properties:
        - A type
        - Value: An internal data representation
        - A set of procedures for interaction with the object ( object’s function, a.f())
    - An object is an instance of a type
- Enumerate():
    - se enumerate to keep track of index and element values: adds a counter to an iterable and returns it in a form of enumerate object.

## Lecture 13: iteration and for loops

- Iteration: basic building block to repeat some code until a condition is met
    - for-loop: iterating over a sequence (set, string, list, tuple or dictionary)
    - Definite iteration: do sth a fixed number of times
    - Process each item in a sequence by executing a set of statements, once for each item in the sequence
- For python’s for loop in a range, example: $\text{}$${\color{lightpink}\text{for}} \space \text{i}\space {\color{lightpink}\text{in}} \space {\color{yellowgreen}\text{range}} ({\color{lightpink}\text{x}})$ generates list and will be iterated through all of its elements so change variable i midway wont affect the number of execution
- Counter and accumulator

```python
number = [1,2,3] # loop sequence: number
for i in number: # loop variable: i
		print(i, end="") # loop body 
										#to end in the same line

# break: finish early and skip all the unexecuted elements
exampleList =[]
for i in exampleList:
		#statements
		break

# continue: skip statements below, and continue next element of loop variable
for i in exampleList:
		#statements
		continue
		#statemetns

# else statement will be executed only when for loop completed without breaking
for i in range(5):
		#statements
		if <condition>:
				#statements
				break
else:
		#statements

x = 3
for i in range(x):
		print(i)
		i = 100 # doesnt change anything 
					  # as the next iteration i is assigned to next element
						# in the list of x
```

## Lecture 14: While-Loops and Loop Invariants

- Definite looping variables
- Always checking the condition, either 0 or 1

```python
while <test_condition>:
		#statements

i = 0
while i < 5:
		i +=1
		print(i) 
```

- Infinite loop: when the condition never becomes false

```python
while count < 3:
		print(count, "is less than 3"
		count += 1 # increment
else:
		print(count, "is not less than 3, ", end = "\\t") # 4 spaces

while True:
		choice = input()
		if choice == 'q' or choice == 'Q':
				break # break out of while loop
```

- Nested while loop:
    
    ```python
    x = 3
    for i in range(x):
    		for j in range(x):
    				print(j)
    		x = 1
    ```
    
    - list(range(x)) returns a list = [ 0, 1, 2, 3], so i is assigned to each elements of the list, changing x only change the new list of range for j

## Lecture 15: Tuples and dictionaries

- Tuple:
    
    - another data type, separated by parentheses()
    - Immutable
    
    ```python
    exampleTuple = (1,2,3,4,5)
    
    # with a single element
    singleElementTuple = ("a") # as same as there is only a string
    type(singleElementTuple)
    >>> str
    
    singleElementTuple = ("a",) # with a comma
    type(singleElementTuple)
    >>> tuple
    
    # Tuple unpacking, nb of elements must as same as the unpacking elements
    exampleTuple = ("HPBD", 19, 0.39, [1,2,3])
    (text, nb, decimal) = exampleTuple
    >>> # text = "HPBD", nb = 19, decimal = 0.39, aList = [1,2,3]
    
    () = exampleTuple
    >>> Error
    
    def exampleFunction(text, nb, decimal, aList):
    		<statements>
    exampleFunction(*exampleTuple)
    >>> # * unpacks all the elements and automatically pass as 4 arguments
    
    # nested tuple works the same way as list
    >>> group1 = (10,20)
    >>> group2 = (30,40)
    >>> group3 = (group1, 50)
    >>> group3
    ((10,20),50)
    
    # tuple concanation are same as list
    
    # delete entire tuple
    >>> my_tuple1 = ("a", "e", "i", "o", "u")
    >>> del(my_tuple1)
    >>> my_tuple1[0]
    #Error not defined
    
    # slicing is as same as list
    
    # if the element is mutable then that element is mutable,
    		# if the list is modified, it has to still be a list afterward
    >>> mytuple = ( 1, 2, 3, [[ 4, 5], 6])
    >>> mytuple[3] = 4
    Error
    >>> mytuple[3][0] = 4
    #ok
    
    # Convert sequence (list or string) to a tuple:
    >>> list2 = [["a", "b", "c"], "Ali", 5]
    >>> tuple(list2)
    (["a", "b", "c"], "Ali", 5)
    
    >>> str1 = "Ali Baba"
    >>> tuple(str1)
    ("A", "l", "i", " ", "B", "a", "b", "a")
    
    # reversed function works the same way with string and list
    # reverse method doesnt work
    >>> t = tuple(reversed(("a", "b", "c", "d")))
    ("d", "c", "b", "a")
    
    # sum
    >>> myTuple = [1,2,3,4]
    >>> sum(myTuple)
    10
    >>> sum(myTuple, 5)
    15 # because sum(mytuple) alone returns 10
    
    # max
    >>> max(("azzz", "bzzz", "z", "Z")
    z # only the first chacter is considered, and a > A
    
    # comparing list and tuple, compare all elements until false, otherwise true
    >>> (2, 3, 4) > (2, 3, 5)
    False # 4 > 5 is False
    >>> (2, 3, 4) == (2, 3, 4)
    True # only true if they are exactly the same
    ```
    
- Dictionary:
    
    - Mutable data type
    - another datatype, each pair separated by curly bracket, key and value separated by colon
    - a set of key/value pairs, called entry
    - accessed values by key
    
    ```python
    # key() and values()
    >>> exampleDict = { "A" : 90, "B" : 80, "C" : 70, "F" : 40}
    
    >>> exampleDict.keys()
    dict_keys(['A', 'B', 'C', 'F']) 
    >>> list(exampleDict.keys())
    ['A', 'B', 'C', 'F']  # displays all the keys in a view obj
    											# This view object points to the original dictionary
    											# so it changes when the orig dict changes
    
    >>>exampleDict.values()
    dict_values([90, 80, 70, 40]) 
    >>> list(exampleDict.values())
    [90, 80, 70, 40]
    
    # accessing values
    >>> "A" in exampleDict
    True
    >>> exampleDict["A"]
    90
    
    # adding and modifying an item 
    >>> exampleDict["D"] = 60 # if the key not existed, adding
    >>> exampleDict
    {'A': 90, 'B': 80, 'C': 70, 'F': 40, 'D': 60} # added at the end
    
    >>> exampleDict["A"] = 95 # if the exists, modifying 
    >>> exampleDict
    {'A': 95, 'B': 80, 'C': 70, 'F': 40, 'D': 60}
    
    # adding and modifying a dict with another
    >>> prime = {2 : "two", 3 : "three", 5 : "five", 7 : "seven"}
    >>> odd = {1 : "one", 3 : "three", 5 : "five", 7 : "SEVEN"}
    >>> prime.update(odd)
    >>> prime
    {2: 'two', 3: 'three', 5: 'five', 7: 'SEVEN', 1: 'one'}
    					# if key already exist, update to new value
    					# else add new entry
    
    # for loop with dict
    		# i refers to the keys only, prime[i] is the value
    for i in odd: 
    		# keys are iterated in order
    for i in sorted(odd.keys()):
    		# keys are iterated in order of ascending of keys
    
    # item function
    >>> prime.items()
    dict_items([(2, 'two'), (3, 'three'), (5, 'five'), (7, 'SEVEN'), (1, 'one')])
    >>> list(prime.items())
    [(2, 'two'), (3, 'three'), (5, 'five'), (7, 'SEVEN'), (1, 'one')] # in pair
    
    # get function
    >>> prime.get(1) # return the value for the corresponding key
    'one'
    
    # convert lists to dictionary
    my_keys = ["Staff ID", "Staff Name", "Department", "Office"]
    my_values = ["100955885", "Ali Baba", "Finance", "Room 1002"]
    myDict = {}
    for i in range(len(my_keys)):
        myDict[my_keys[i]] = my_values[i]
    print(myDict)
    
    # another way
    exampleDict = dict([(1, 'a'), (2, 'b'), (3, 'c')])
    
    # unpacking for dictionary doesnt works the way as unpacking tuples
    def exam_sum(midterm = 0, final = 0):
        print(midterm + final)
    grade = {"midterm": 20, "final": 5}
    
    exam_sum(**grade) # exam_sum(midterm : 20, final : 5)
    exam_sum(*grade)  # same as exam_sum(*grade.keys()) 
    									# and exam_sum( "midterm", "final")
    exam_sum(*grade.values()) # exam_sum( 20, 5)
    
    # ** unpack by pair, and * unpack the keys
    ```
    

## Lecture 16: Algorithm Design

- Algorithm is a step-by-step procedure which defines a set of instructions to be executed in a certain order to solve problem and get the desired output.
    - Independent of underlying language
    - Characteristics of algorithms:
        - Unambiguous
        - Input
        - Output
        - Finiteness
        - Feasibility
        - Independent
- Most efficient for a given problem: algorithm with the least execution time
- Factors that affect execution time:
    - Amount of data
    - Type of hardware
    - Programming language and compiler used
    - …
- Big-O notation: used to describe the complexity by worse case scenario, how many steps required to execute the algorithm between the inputs. Time = sum of time for all statements
    - Constant-time algorithm: O(1) or order 1, no matter the size of input same nb of steps
        - for basic operations
    - Linear-time complexity: O(n) or order of n
    - Logarithm-time complexity: O(log(n))
    - O(nlog(n))
    - ….

## Lecture 17: Sorting

- Selection sort: O(n^2)
    
    - First unsorted compared to all the rest, if bigger, swap
    
    ```python
    def selectionSort(array, size):
        for ind in range(size):
            min_index = ind
     
            for j in range(ind + 1, size):
                # select the minimum element in every iteration
                if array[j] < array[min_index]:
                    min_index = j
            # swapping the elements to sort the array
            (array[ind], array[min_index]) = (array[min_index], array[ind])
    ```
    

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a89f9b6f-1374-4e0d-902d-6663344150a3/Untitled.png)

- Merge Sort: O(n*log(n))
    
    - Keep divide the array to 2 subarrays til only 1 item left
    
    ```python
    def mergeSort(arr, l, r):
        if l < r:
            # Same as (l+r)//2, but avoids overflow for
            # large l and h
            m = l+(r-l)//2
     
            # Sort first and second halves
            mergeSort(arr, l, m)
            mergeSort(arr, m+1, r)
            merge(arr, l, m, r)
    ```
    
- Quick Sort: O(n^2)
    
    - Choose a pivot number, can be first or last or median; then divides 2 subarrays, one for values bigger than pivot and one for smaller.
    
    ```python
    # Function to find the partition position
    def partition(array, low, high):
        # choose the rightmost element as pivot
        pivot = array[high]
        # pointer for greater element
        i = low - 1
        # traverse through all elements
        # compare each element with pivot
        for j in range(low, high):
            if array[j] <= pivot:
                # If element smaller than pivot is found
                # swap it with the greater element pointed by i
                i = i + 1
                # Swapping element at i with element at j
                (array[i], array[j]) = (array[j], array[i])
        # Swap the pivot element with the greater element specified by i
        (array[i + 1], array[high]) = (array[high], array[i + 1])
        # Return the position from where partition is done
        return i + 1
     
    # function to perform quicksort
    def quickSort(array, low, high):
        if low < high:
            # Find pivot element such that
            # element smaller than pivot are on the left
            # element greater than pivot are on the right
            pi = partition(array, low, high)
            # Recursive call on the left of pivot
            quickSort(array, low, pi - 1)
            # Recursive call on the right of pivot
            quickSort(array, pi + 1, high)
    ```
    
- Insertion sort:
    
    - Pick each item one at a time, and insert it where it is less than the right one and smaller than the left one

## Lecture 18: Search

- Linear search:
    
    - Compare each and every item
- Binary Search:
    
    - Requires the array to be sorted beforehand
    - Begin with the mid element of the whole array as a search key.
    - If the value of the search key is equal to the item then return an index of the search key.
    - Or if the value of the search key is less than the item in the middle of the interval, narrow the interval to the lower half.
    - Otherwise, narrow it to the upper half.
    - Repeatedly check from the second point until the value is found or the interval is empty.
    
    ```python
    def binarySearch(arr, x, low, high):
        while(low != high):
             mid = (low + high)/2
             if (x == arr[mid])
    		         return mid
             elif (x > arr[mid]) # x is on the right side
                 low = mid + 1
             else:                  # x is on the left side
                 high = mid - 1
    ```
    

## Lecture 19: Recursion

- A methods of solving a problem where the solution depends on solutions to smaller instance of the same problem
- Base Case: stopping condition-case
- Recursive case:
    - for a list, the recursive case is always connecting the first item and the function(rest of the list)

1. Towers of Hanoi:
    
    - Tower of Hanoi is a mathematical puzzle where we have three rods and n disks.
        
    - The objective of the puzzle is to move the entire stack to another rod
        
        1. Only one disk can be moved at a time.
            
        2. Each move consists of taking the upper disk from one of the stacks and placing it on top of another stack i.e. a disk can only be moved if it is the uppermost disk on a stack.
            
        3. No disk may be placed on top of a smaller disk.
            
    
    ```python
    def TowerOfHanoi(n , source, destination, auxiliary):
        if n==1:
            print ("Move disk 1 from source",source,"to destination",destination)
            return
        TowerOfHanoi(n-1, source, auxiliary, destination)
        print ("Move disk",n,"from source",source,"to destination",destination)
        TowerOfHanoi(n-1, auxiliary, destination, source)
    ```
    
2. Fibonacci Tower:
    
    ```python
    def fibonacci(N):
        if N == 1:
            return 0
        if N == 2:
            return 1
        return fibonacci(N - 1) + fibonacci(N - 2)
    ```
    
3. Pascal’s triangle:
    
    ```python
    def PascalTriangle(n):
       trow = [1]
       y = [0]
       for x in range(n):
          print(trow)
          trow=[left+right for left,right in zip(trow+y, y+trow)]
       return n>=1
    ```
    

## Lecture 21: OOP

- Concepts:
    - Inheritance: The transfer of the characteristics of a class to other classes that are derived from it.
    - Polymorphism
    - Abstraction: shows only important attributes while hiding unnecessary details from the user. It helps in reducing programming complexity and increase efficiency.
        - The abstraction is done during the design level of a system and encapsulation is done when the system has been implemented
    - Encapsulation: a programming technique that binds the class members together and prevents them from being accessed by other classes. Restricted access to Class members: variables and methods To keep variables and methods safes from outside interference and misuse.
- Object is an instance of a class, with different attributes and methods from one another
    - Instance: An individual object of a certain class.
- Class: A user-defined prototype for an object that defines a set of attributes that characterise any object of the class. The attributes are data members (class variables and instance variables) and methods, accessed via dot notation.
- Variables:
    - Class variable: A variable that is shared by all instances of a class. Class variables are defined within a class but outside any of the class's methods. Class variables are not used as frequently as instance variables are.
    - Instance variable: A variable that is defined inside a method and belongs only to the current instance of a class.
    - Data member
- Function overloading: The assignment of more than one behaviour to a particular function. The operation performed varies by the types of objects or arguments involved.
- Operator overloading: The assignment of more than one function to a particular operator.
- When inside a class: method, outside of the class: function

## Lecture 22: Design classes and constructors

- Constructions:
    
    - Constructor is called whenever new object is initialized
        
        - Default constructor: no argument to be passed
            
            ```python
            def __init__(self):
            ```
            
        - Parameterised constructor: requires multiple parameters with self
            
            ```python
            def __init__(self, name, age):
            ```
            
    - Constructors are automatically created by Python only default constructor
        
    - An object cannot be created if the class doesn’t have a constructor
        
    
    ```python
    class LivingThing():
        """
    				class specification
    				instance is an living thing
    				children classes can be mammals, fish, homo sapiens,...
    		"""
    		nbOfLivingThings = 0   #class attributes
    		limbs = 4
    
        def __init__(self, name, nbOfLimbs, nbOfHearts): # Constructor with function overloads
    												# sequence of actions required so that factory constructs an object
    				self.name = name
    				self.nbOfLimbs = nbOfLimbs
    				self.nbOfHearts = nbOfHearts
    		def Breath():
    				<statements>
    
    self.variable # refers to the instance's variable
    Class.variable # refers to the class's value
    ```
    
- Instantiation:
    
    ```python
    dog = LivingThing()
    print(dog) # print the memory address of the object
    print(LivingThing) # print the memory address class
    ```
    
    - New object created is different from another object even though created from the same class
- Deleting an object:
    

```python
del <objName>
```

- Convert an object to a string when called
    
    - if not, pointer to the object is a memory address
    
    ```python
    def __str__(self):
    		return "welcome to " + self
    print(objName)
    ```
    
- Built-in class functions:
    

![Screenshot 2022-12-28 at 17.49.23.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/754d44a5-9e81-4c43-a88b-0882aaabc429/Screenshot_2022-12-28_at_17.49.23.png)

- Built-in class attributes:

![Screenshot 2022-12-28 at 17.49.12.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1c2262a6-a412-4d55-b5f7-a9bb014a4e31/Screenshot_2022-12-28_at_17.49.12.png)

- Invariants

## Lecture 23: Subclasses and inheritance

- Inheritance:
    
    ![Screenshot 2022-12-28 at 17.53.28.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/35c44007-ba12-4380-adc2-0cd536efe37f/Screenshot_2022-12-28_at_17.53.28.png)
    
    - Simple inheritance: a process by which one child class (subclass) takes on the attributes and methods of another, parent (base/super) class
        
        - newly formed classes that can override or extend the attributes and methods of parent classes
            
            ```python
            class Car:
            		def __init__(self, color, year):
            				self.color = color
            				self.year = year
            
            class Bus(Car):
            		def __init_(self, color, year, brand):
            				super().__init__(color, year) #super refers to immediate parent class
            				self.brand = brand
            
            ```
            
    - Multiple inheritance: a class is derived from more than one base class
        
        ```python
        class <childClass>(<parentClass1>, <parentClass2>):
        		# body
        class Bus(Car, Van)
        ```
        
        - The properties and methods of all the base classes are inherited into the derived class.
        - First come first serve, so if the name of methods/attributes are repeated then the first parent’s is used
    - Deadly diamond of death (hybrid):
        
        ![Screenshot 2022-12-28 at 18.03.19.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/81b5331d-3448-4881-a98a-aad5f667bffe/Screenshot_2022-12-28_at_18.03.19.png)
        
        - Class B and C inherits from class A, but class D inherits from both B and C
    - ## Method resolution order:
        
    - Check relationship:
        
        ![Screenshot 2022-12-28 at 18.05.32.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/303a4190-7f2a-4182-8344-75754d0938db/Screenshot_2022-12-28_at_18.05.32.png)
        

## Lecture 24: Operator and function overloading

- Operator overloading:
    
    - Change how objects behave under operations like +, -, *, /, comparision,…
        
        ```python
        class Vector():
        		def __init__(self,x,y):
        				self.x = x
        				self.y = y
        		def __add__(self, another):
        				return Vector(self.x+another.x, self.y+another.y)
        vector1 = Vector()
        print(dir(vector1))   # returns all properties and methods of the 
        										  # specified object, without the values
        ```
        
- Function overloading
    
    - - (args) passes variable number of non-keyworded arguments as a list
            
            ```python
            def sum_all (*prices):
            		total = 0
            		for i in prices:
            				total += i
            		print( "Total is ", total)
            sum_all (100, 200)
            sum_all (100, 200, 300)
            ```
            
    - ** (kwargs) passes variable number of keyword arguments dictionary to function on which operation of a dictionary can be performed
        
        ```python
        def sum_sales(**monthly_sales):
        		total = 0
        		for key, value in monthly_sales.items ():
        				total += int (value)
        		print ("Total is " total)
        sum_sales (Jan=100, Feb=200) 
        sum_sales (Jan=100, Feb=200, March=300)
        ```
        
    - *args and **kwargs make the function flexible.
        
- Encapsulation: Restrict access to methods and variables to prevent data modification
    
    - Private attributes are prefixed with __
    
    ```python
    class Meat():
        def __init__(self):
            self.__price = 20
        def sell(self):
            print(f"1  + {self.__price}")
        def ChangePrice(self, new):
            self.__price = new
    
    chicken = Meat()
    chicken.__price = 25 # this is ignored
    chicken.ChangePrice(15) # this modify the private attribute
    ```
    
- Polymorphism:
    
    - Methods in child class has the same name as the methods in the parent class
    - Child class modifies the method it has inherited from the parent class
    
    ```python
    class Vehicle:
    		def show(self):
    				print("I am from the base class")
    
    class Car(Vehicle):
    		def show(self):	# this modifies the method for Car objs
    				Vehicle.show(self) # call parent's method
    				print("I am from the derive class")
    ```
    

## Lecture 25:

- Numpy
- Panda
- Matlib

Week 15 not in final exam