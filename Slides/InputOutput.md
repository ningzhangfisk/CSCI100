## 3.3.6 Input Output
### 3.3.6.1 What is I/O?
+ In computing, input/output (I/O, or informally io or IO) is the communication between an information processing system, such as a computer, and the outside world, possibly a human or another information processing system.
+  Inputs are the signals or data received by the system.
+  Outputs are the signals or data sent from it.
### 3.3.6.2 Output in Python
+ Printing to the Screen
~~~~
# example 1
print("Hello World!")
# example 2
# see the space after hello, why?
name = "John"
print("Hello " + name)
~~~~

### 3.3.6.3 Input in Python
+ What if we want to replace the strings used in the examples above with anything the user entered?
+ We can use `input` function to prompt the user to type something.

~~~~
# see the \n (you can also use a space) in the end of the string, why?
name = input('What is your name?\n')
print("Hello " + name)
~~~~
+ When we run the program above, a string `What is your name?` will be displayed on the screen.
+ Once the user types their entry and hits the "enter" key...
+ The string the user enters will be stored in this variable `name` as a `string`.

### 3.3.6.4 Communicating With User
+ `input()` lets user input text.
+ `print()` outputs text to user.
+ `input()` always gives a string; if want number, use `int()` or `float()` as appropriate.

~~~~
name = input("What is your name?")
print("Hi there, " + name)
age = int(input("How old are you?"))
print("Next year, you'll be " + (age + 1) + "years old.")
~~~~
### Summary of I/0
+ What is it?
  - User providing input and receiving output
+ Why is this important?
  - Many programs and apps need user input, and based on input, program provides output
+ How (in Python)?
  - input(): get input from user
  - print(): show output to user
## 3.3.7 Comparison Operators and Conditionals

![3-6](../Resources/3-6.png)

+ when `order_cost = 26.95`, which statement should we execute?
  - `print("Shipping is free!")`
  - `print("Shipping is $5.99")`

![3-7](../Resources/3-7.png)
