# Computer science

## Data structures

### What is the purpose of a list (array in some programming languages) data structure? Name some methods of it!

> A list is a data structure which can hold a seemingly unlimited amount of data. In Python, it can hold any arbitrary 
> data.
> Some methods are: ``append()``, ``indexof()``, ``remove()``, ``sort()``, ``reverse()``, etc.

### What is the difference between a list/array and a set?

> Lists are order and changeable, allowing duplicates.
> Sets are unordered, unchangeable, unindexed and only allow unique members.

### What is the purpose and methods of a dictionary/map data structure?

> Dictionaries hold data in key-value pairs. It allows faster lookup and retrieval of values based on their associated 
> keys and also useful if we need to store and retrieve data in an unordered manner.
> Methods include: ``keys()``, ``values()``, ``items()``, ``update()``, ``remove()``, ``pop()``, ``popitem()``, ``clear()``

## Algorithms

### Fibonacci sequences. Write a method (or pseudo code), that generates the Fibonacci sequences.

```python
def fibonacci(n): # Gets the Nth fibonacci number
    if n <= 1:
        return n
    else:
        return fibonacci(n - 1) + fibonacci(n - 2)
```

### How do you find a max value in a list/array if you can’t use any built-in functions?

```python
def find_max_value(array):
    max_num = array[0] if array else None
    for num in array[1:]:
        max_num = num if num > max_num else max_num
    return max_num
```

### How do you find the average of values in a list/array if you can’t use any built-in functions?

```python
def find_average_value(array):
    sum_num = 0
    length = 0
    for num in array:
        sum_num += num
        length += 1
    return sum_num / length
```

### Explain an algorithm which sorts a list!

> ``bubble sort``, ``quick sort``

## Programming paradigms - procedural

### What is the call stack?

> A call stack is a FILO data structure, meaning the first thing that got is going to be the first get out. It keeps 
> track of functions, variables, object, etc. while the program is running. 

### What is “Stack overflow”?

> Stack overflow happens, when the allocated memory is being used up by the program. It can happen, when a 
> recursive function is written poorly.

### What are the main parts of a function?

> ``def`` keyword, function name, function body

## Programming languages - Python

### How do you use a dictionary in Python?

> It is used to store key-value pairs. See the rest above.

### What does it mean that an object is immutable in Python?

> It means the object can't be changed. SO if we want to change a string, we are not changing that specific string, but 
> we are creating a new string with the changes.

### What is conditional expression in Python?

> It's also called ternary operator. It can be used to create single line if-else statements.

### What are different types of arguments in Python?

> The main types of arguments in Python are ``positional``, ``keyword``, ``default``, ``*args``, ``**kwargs`` 

### What is variable shadowing? (context: variable scope)

> Variable shadowing happens when a variable is reintroduced in another variable scope, which may create confusion and errors.

### What can happen if you try to delete/drop/add an item from a List, while you are iterating over it in Python?

> Changing a list while iterating through it can cause unwanted and unexpected errors.

### What is the "golden rule" of variable scoping in Python (context: LEGB)? What is the lifetime of variables?

> The lifetime of a variable is based on the smallest scope it is in. So a variable declared inside a function will 
> only hold up until the function finished running. The golden rule refers to the levels of variable scopes the program 
> is looking for a variable starting from local to enclosed, global, then built-in.

### If you need to access the iterator variable after a for loop, how would you do it in Python?

> We can access it by simpy calling it, however we can only use it's last value. If we want to use multiple of its 
> values, we can save it inside a list or some other data structure.

### What type of elements can a list contain in Python?

> Basically any arbitrary data structures.

### What is slice operator in Python and how to use?

> The slice operator lets us create substrings or sublists.

### What arithmetic operators (+,*,-,/) can be used on lists in Python? What do they do?

> In Python only the ``+`` and the ``*`` operator can be used on lists. The first one adds elements into the list, the 
> other one multiplies the list's elements the defined times.

### What is the purpose of the in and not in membership operators in Python?

> We can check if some data is in or not in a list, dictionary, etc. It save us from looping through data structures.

### What does the + operator mean when used with strings in Python?

> It is used for string concatenation, meaning it joins two or more strings into one.

### Explain f strings in Python!

> An f string lets us use variables, expressions or objects in string definitions.
```python
name = 'Gina'
age = 32
print(f'{name} is {age} year(s) old.')
```

### Name 4 iterable types in Python!

> ``list``, ``string``, ``dictionary``, ``set``

### What is the difference between list/set/dictionary comprehension and a generator expression in Python?

> With comprehension the whole data structure is created and stored in memory, while generator expression give us one 
> data at a time when it is called, making it a lot more memory efficient.

### Does the order of the function definitions matter in Python? Why?

> Yes, it does. Since Python is an interpreted language, meaning the code is executed sequentially, from top to bottom.
> However if we use the ``if __name__ == '__main__'`` construct, this 'flaw' can be evaded.

### What does unpacking mean in Python?

> Unpacking refers to the practice of assigning values to multiple variables at the same time.
> Ie.: ``x, y = (10, 15)``, ``year, month, day = [2023, 12, 14]``

### What happens when you try to assign the result of a function which has no return statement to a variable in Python?

> It will receive a NoneType value.