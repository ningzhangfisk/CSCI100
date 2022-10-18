# 3.3.12 Functions
## 3.3.12.1 Introduction
+ A **function** is a block of statements that return the specific task.
+ The idea is to put some commonly or repeatedly done tasks together and make a function so that instead of writing the same code again and again for different inputs.
+ we can do the function calls to reuse code contained in it over and over again. 
## 3.3.12.2 Syntax

![function Syntax](https://media.geeksforgeeks.org/wp-content/uploads/20220721172423/51.png)


## Creating a Python Function (with no arguments or return value)
We can create a  Python function using the `def` keyword.

~~~~
# a simple Python function
def func():
  print("Hello")
~~~~

+ Calling a  Python Function
After creating a function we can call it by using the name of the function followed by parenthesis containing parameters of that particular function.

~~~~
# A simple Python function
def func():
  print("Hello")
 
 
# Driver code to call a function
func()
~~~~

### Defining and calling a function with arguments and/or return value(s)
+ Arguments are the values passed inside the parenthesis of the function. A function can have any number of arguments separated by a comma.
+ Return values are the results a function gets and returns to the user.
+ Syntax
~~~~
def function_name(parameter: data_type):
    """Docstring"""
    # body of the function
    return expression
~~~~
+ Example
In the following function named **add**, it has two parameters **num1** and **num2**, and returns **num3**.
~~~~
def add(num1, num2):
  """add two numbers"""
  num3 = num1 + num2
  
  return num3
  
# test code
num1, num2 = 5, 15
ans = add(num1, num2)
print("The addition of ", num1, "and", num2, "results", ans)
~~~~

### Default arguments
+ A default argument is a parameter that assumes a default value if a value is not provided in the function call for that argument. The following example illustrates Default arguments. 
+ Example

~~~~
# Python program to demonstrate
# default arguments

def myFun(x, y=50):
    print("x: ", x)
    print("y: ", y)
 
 
# test code (We call myFun() with only one argument)
myFun(10)

# test code (We call myFun() with two arguments)
myFun(10,20)
~~~~

### Keyword arguments
+ The idea is to allow the caller to specify the argument name with values so that caller does not need to remember the order of parameters.
+ Example

~~~~
# Python program to demonstrate Keyword Arguments
def student(firstname, lastname):
    print(firstname, lastname)
 
 
# Keyword arguments
student(firstname='John', lastname='Doe')
student(lastname='Doe', firstname='John')
~~~~


### Docstring
+ The first string after the function is called the Document string or Docstring in short. This is used to describe the functionality of the function. The use of docstring in functions is optional but it is considered a good practice.

+ The below syntax can be used to print out the docstring of a function:

~~~~
print(function_name.__doc__)
~~~~

+ Example

~~~~
# A simple Python function to check

def add(num1, num2):
  """add two numbers"""
  num3 = num1 + num2
  
  return num3

# test code to call the function
print(add.__doc__)
~~~~


### Return statement in Python function
+ The function return statement is used to exit from a function and go back to the function caller and return the specified value or data item to the caller.

+ Syntax

~~~~
return [expression_list]
~~~~

+ The return statement can consist of a **variable**, an **expression**, or a **constant** which is returned to the end of the function execution. If none of the above is present with the return statement a None object is returned.
+ Example 1: return one value

~~~~
def square_value(num):
    """This function returns the square
    value of the entered number"""
    return num**2
 
 
print(square_value(2))
print(square_value(-4))
~~~~

+ Example 2: return multiple values (a tuple)

~~~~
# A Python program to return multiple 
# values from a method using tuple
  
# This function returns a tuple
def fun():
    name = "John Doe"
    age   = 20
    return name, age;  # Return tuple, we could also write (name, age)
  
# test code to test above method
name, age = fun() # Assign returned tuple
print(name)
print(age)
~~~~
