# Python Documentation

#### Index:
[Data Types:](https://carlover101.github.io/python-docs/#data-types)
- [Strings](https://carlover101.github.io/python-docs/#strings)
- [Integers](https://carlover101.github.io/python-docs/#integers)
- [Floats](https://carlover101.github.io/python-docs/#floats)
- [Lists](https://carlover101.github.io/python-docs/#lists)

[Variables:](https://carlover101.github.io/python-docs/#variables)

[Conditional Statements:](https://carlover101.github.io/python-docs/#conditional-statements)
- [If, Else Statements](https://carlover101.github.io/pgython-docs/#if-else-statements)
- [Try and Except Statements](https://carlover101.github.io/python-docs/#try-and-except-statements)

[Loops:](https://carlover101.github.io/python-docs/#loops)
- [While Loops](https://carlover101.github.io/python-docs/#while-loops)
- [For Loops](https://carlover101.github.io/python-docs/#for-loops)

[Functions:](https://carlover101.github.io/python-docs/#functions)

[Files:](https://carlover101.github.io/python-docs/#files)

[Importing Libraries:](https://carlover101.github.io/python-docs/#importing-libraries)

#### The source file can be found at [this link](https://carlover101.github.io/python-docs/index.md)

## Data Types:

### Strings:

- A string contains a set of characters that can be manipulated to do several things such as, print statements and store information.
  - Strings start and end with " or ' (double or single quotations), but you cannot start with one and end with the other.

##### Example 1:

```
  print("Hello world!")
```
- This string starts and ends with "
  - In this case, the string is: "Hello world!"

##### Example 2:

```
  answer = input('What is your name? ')
```
- This string starts and ends with '
  - In this case, the string is: 'What is your name? '

### Integers:

- An integer is like a string except it can only have whole numbers and it doesn't use quotations.
  - Integers can be divided ( using / ), added together ( using + ), subracted from one another ( using - ), multiplied ( using * ), and so on.

##### Example 1:

```
  a = "1"
  b = int(a)
```
- *a* is equal to the string "1", but it is not an integer. While, *b* is equal to the integer of a, so 1, and can be used as so.

##### Example 2:

```
  a = "4"
  b = int(a)

  print(a / 2)
  print(b / 2)
```
- *a* will give you an error because Python thinks you are trying to divide a string. But, *b* will print 2 because it is an integer and functions as so.

### Floats:

- A float is like an integer, except it is able to use decimals as well as whole numbers.

##### Example 1:

```
  a = "1.5"
  b = int(a)
  c = flaot(a)
```
- In this example, *b* will not assign, but error out because the int() function does not take decimals, and *c* will turn the string "1.5" into 1.5.

##### Example 2:

```
  a = "4.5"
  b = int(a)
  c = float(a)

  print(a * 2)
  print(b * 2)
  print(c * 2)
```

- In this example, multiplying *a* by 2 will not error out, but instead of printing 9, which is the correct answer, it will just print the string "4.5" twice. As with the last example, assigning *b* will not work because the int() function does not work with decimal points. But, *c* will work as intended and print 9.

### Lists:

- Lists are used to store a lot of the previous types of data in one referenceable name.

##### Example 1:

```
  list1 = ["word1", 1, 1.0]

  print(list1[0])
```

- In this example, the items in the list are being assigned ahead of time, and separated with commas.
  - As shown with the print statement, the first item of the list is being printed. To reference specific items in a list, you take the item place, and subtract one number.

##### Example 2:

```
  number = 1.0
  list1 = ["word1", 1]

  list1.append(number)

  print(list1[2])
```

- In this example, the **.append()** option is used to add another item to the list, since it wasn't there in the beginning.

## Variables:

- Variables are words or recognizable arrangements of characters that can be assigned a specific value that can be referenced later or changed.
  - Variables are assigned using the = symbol, and can contain letters and numbers, but must never start with a number.

##### Example 1:

```
  var1 = "Hi"
```

- In this example, the variable is *var1* is assigned the string "Hi".

##### Example 2:

```
  var1 = "Hello "
  var2 = "World!"
  var3 = var1 + var2

  print(var3)
```

- This example uses the string combining feature to take the two variables and combine them into one, and then print it.

## Conditional Statements:

### If, Else Statements:

- An if, then statement is used to execute code when a certain thing is true.

##### Example 1:

```
  a = 1
  b = 2

  if a == b:
    print("a is equal to b. ")

  else:
    print("a is not equal to b. ")
```

- In this example, the if, then statement is being used to detect if *a* is equal to *b* or not, and to print something depending on the outcome.

##### Example 2:

```
  a = 1
  b = 2
  c = 3

  if a == b:
    print("a is equal to b. ")

  elif a == c:
    print("a is equal to c. ")
  
  else:
    print("a is not equal to b or c. ")
```

- If this example, the code demostrates another use of the if, else conditional statement, the **elif** statement. 
  - This gives the coder the ability to have several things checked before ending the if, else statement.
  - The elif statement can be used as many times as necessary.

### Try and Except Statements:

- The try and except statement is used to attempt to run a piece of code, and if it doesn't work, do something else.

##### Example 1:

```
  a = "1.0"
  
  try:
    b = int(a)
  
  except:
    print("b is not an integer or it contains a decimal point.")
```

- In this example, try and except is used to try to convert *a* or "1.0" into an integer, but since it contains a decimal point, it fails and moves on to the except statement.

##### Example 2:

```
  a = "1.0"
  b = "1.5"

  try:
    c = int(a)

  except:
    print("a is not an integer or it contains a decimal point.")
    c = int(b)

  finally:
    print("a and b are not integers or they contain a decimal point.")
```

- In this example, the try and except statement is used to attempt to convert *a* or "1.0" into an integer, but since it has a decimal point, it doesn't work, and the except attempts to convery *b* or "1.5" into an integer, but since it also contains a decimal point, it didn't work as well.

  - Finally is used at the end as the finishing statement to say, if nothing else works, do this.

## Loops:

- A loop is a function in python that run the same piece of code more than once in the same spot.

### While Loops:

- A while loop is used to run the same piece of code as many times as something is true.

##### Example 1:

```
  while True:
    print("This is true!!!!")
```
- This example uses the version of the while loop often known as the "forever loop" because it will coninue to run indefintely unless told otherwise.

##### Example 2:

```
  a = 10

  while a >= 1:
    a = a - 1
    print("a is greater than 0")
```

- In this example, the while loop is used to print that the variable *a* is greater than 0 while it is. It will stop after *a* reached 0.

### For Loops:

- A for loop runs a piece of code a specific amount of times.

##### Example 1:

```
  number = 10

  for i in range(number):
    print(i)
```

- This example uses the range function of the for loop to run the piece of code the number of times specified in the parantheses.

##### Example 2:

```
  list1 = ["str1","str2","str3"]

  for item in list1:
    print(item):
```

- In this example, the for loop is assigning the variable *item* to the corresponding item in *list1* and printing it.

## Functions:

-  A function is a variable or a memorable name that can be referenced at a later time to run a piece of code.

##### Example 1:

```
  def function1():
    print("This is a function.")
    print("This function does two things in one line!")

  function1()
```

- This example defines the function at the beginning, and then runs it at the end.

##### Example 2:

```
  def function1(word1,word2):
    print(f"Normal: {word1} {word2}")
    print(f"Backwards: {word2} {word1})

  function1("Green","Giraffe")
```

- In this example, the function is defined as usual, but it also requires the input of two varibles that are used in the code as shown above.

## Files:

- Python can be used to sort through text files and read and change lines in those files.

##### Example 1:

```
  f = open("file.txt")

  for line in f:
    if "the" in line.lower():
      print("The word 'the' appear in the file.")
```

- This example just goes through the text file line by line, and if the word "the" appears in the line, it will print the selected string.

##### Example 2:

```
  f = open("file.txt", "w")

  for line in f:
    f.write(line + "Hello!")
```

- In this example, "w" is used to signify that the user wants to write to the file.
  - The program takes each line and adds "Hello!" to the end and writes it to the end of the file.

## Importing Libraries

- Importing libraries in Python gives the user many more options to work with that are not normally possible with them.
  - Libraries are imported using **import** and then the library name, such as **time** or **os**, which are some of the more commonly used.

##### Example 1:

```
  import time

  print(f"Current time: {time.time()})
  time.sleep(1)
  print(f"Time 1 second later: {time.time()}")
```
- In this example, the **time** library is imported and used to display the current time and wait one second before displaying the time again.

##### Example 2:

```
  from time import sleep
  from os import system as sys

  print("Hi)
  sleep(1)
  sys("clear")
  print("Bye")
```

- This example shows the use of importing specific functions from libraries, **sleep** in this case, and naming those imported libraries, turning **system** into **sys**.
  - This is jsut a simple example of the many libraries that can be used in Python.
