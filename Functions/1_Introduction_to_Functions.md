**Author:** S Sandeep Pillai.

**Edits:** Ashley TR, Pranav Shridhar

***

# Functions

**A function (or method) is defined as a named encapsulation of a specific set of instructions in a program.** 

In normal English, it can be considered as a package/collection of lines of code that will be executed each time you 'call' it later on in your program. So this splits the program into "modules" or chunks that each person can work on separately.

Now before we get into the boring theory, let us delve into how we can use functions in Python.

## Syntax

There are two kinds of functions within python: 
1) Built-In Functions 
2) User Defined Functions

Implicit Functions are predefined functions within Python, or a module linked through Python. We shall focus on Explicit Functions 
for now.

### Stop it with the Theory! 

Okay, fine, so a function needs to be defined beforehand for it to be used later in the program. To define a function, we need
to use the following keywords:

```python
def function-name ( Argument-1, Argument-2, ... Argument-N ):   #Make sure you don't forget the colons in the end! (' : ')
    
    Line 1
    Line 2:
        Line 2.1
        Line 2.2
        Line 2.3:
            Line 2.3.1
            Line 2.3.2
    Line 3
    Line 4

#End of "function-name".
``` 
Here, we use the keyword *`def`* to invoke the function definition clause so that the interpreter will know the following line
contains the definition of a function. To use this function later, simply follow the syntax:

```python

function-name( Arg1, Arg2, ArgN ):  #This will execute Lines 1 to 4 once.

```

Now let us look at an example where functions can prove very useful in your program you will be writing.

Suppose we are developing a college-assistant application, with a wide range of tools such as a 'timetable manager', 'announcements viewer', 'test date reminders', and the very popular 'Class Bunker Calculator', it would be convenient to enclose each functionality within its own functions.

## Example Program:

But for now, let us diverge from that and look at how we can design a simple arithmetic calculator:

```python

def add(num1, num2):         # This function will take in 2 variable arguments.
        sum = num1 + num2   # These arguments are added together and stored in the variable 'sum'.
        print(sum)          # The variable sum is then printed onto the console.
        
def subtract(num1, num2):
        print( num1 - num2 )    # Another method would be to simply print out the compound statement as shown, avoiding the 
                                # the usage of a variable such as 'sum', helping reduce memory usage.

def multiplication(num1, num2):
        multip = num1 * num2
        print(multip)
        
def division(num1, num2):
        div = num1 / num2
        return(div)    # We can instead return the value, if we wish to use this value for other purposes in the program.
        
def odd_even_checker(num1):
        if num1 % 2 == 0:       # We can implement an if clause in a function, as shown here.
            print("EVEN")       
        else:
            print("ODD")
        


```
We can now call any of the functions defined above as many times as we want later in the program. Let us assume later in the code, we need to multiply 42 and 25. We can simply "CALL" the `multiplication` function in the lines below instead of writing the entire sequence of code again.
```python3
 
multiplication( 42, 25 ) # Here, 42 is assigned to num1 and 25 is assigned to num2.

```

This will give us the output :


```
1050
```

**NOTE: Useful Built-In functions are discussed in the other modules of this 'textbook' ** 

## Advantages of using a function:

  * It allows for a significantly shorter length of the program code. 
  * You can reuse the code repeatedly (by calling the function) instead of rewriting the same set of instructions again.
  * Significantly improves code debugging - it will allow you to pinpoint an error to a specific code block.
  * If a certain function breaks during development, you can still run the rest of the program without issues (by commenting out that particular function).
  * Allows division of labour: each member can work on a separate function without conflicting code.

***
## [Interesting? You might also be interested in the compound and built-in functions](https://github.com/vhawk19/Py_Primer/blob/master/Functions/2_BuiltIn_%26_Composition_Functions.md)
