# 3.3.10 Selection
+ There comes situations in real life when we need to make some decisions and based on these decisions, we decide what should we do next. Similar situations arise in programming also where we need to make some decisions and based on these decisions we will execute the next block of code. Decision-making statements in programming languages decide the direction of the flow of program execution. 
+ In Python, `if` statements will be used for decision making.
+ We will learn four different types of `if` statements in the section.
  - `if` statements
  - `if else` statements
  - `nested-if` statements
  - `if elif else` statements

# 3.3.10.1 `if` statement
+ if statement is the most simple decision-making statement. It is used to decide whether a certain statement or block of statements will be executed or not i.e if a certain condition is true then a block of statement is executed otherwise not.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/if-statement.jpg" alt="if statement" style="width:300px; height:400px">


+ Syntax

~~~~
if condition:
   # Statements to execute if
   # condition is true
~~~~

+ Here, the condition after evaluation will be either true or false. if the statement accepts boolean values – if the value is true then it will execute the block of statements below it otherwise not. We can use condition with bracket `()` also.
+ As we know, python uses indentation to identify a block. So the block under an if statement will be identified as shown in the below example:

~~~~
if condition:
   statement1
statement2

# Here if the condition is true, if block 
# will consider only statement1 to be inside 
# its block.
~~~~

+ Example
  - As the condition present in the `if` statement is true. So, the if block is executed.
  - What is the result if we change `i` to 10?
  - the `print("done")` statement is NOT in the `if` statement, so it will always be executed.
~~~~
# python program to illustrate If statement
  
i = 20
  
if (i > 15):
    print(i, "is less than 15")
    
print("done")
~~~~

## 3.3.10.2 `if else` statement
+ The `if` statement alone tells us that if a condition is true it will execute a block of statements and if the condition is false it won’t. But what if we want to do something else if the condition is false. Here comes the `else` statement. We can use the `else` statement with `if` statement to execute a block of code when the condition is false. 


<img src="https://media.geeksforgeeks.org/wp-content/uploads/if-else.jpg" alt="if else statement" style="width:300px; height:400px">


+ Syntax
~~~~
if condition:
    # Executes this block if
    # condition is true
else:
    # Executes this block if
    # condition is false
~~~~

+ Example
  - The condition is false, so the `else block` will be executed.
  - What if we change `i` to 10?
  - the `print("done")` statement is NOT in the `if-else` statement, so it will always be executed.
~~~~
# python program to illustrate if else statement
  
i = 20
if (i < 15):
    print("i is smaller than 15")
    print("i'm in if Block")
else:
    print("i is greater than 15")
    print("i'm in else Block")
print("done")
~~~~

+ Practice: Write a program to ask the user to provide an integer and find out the number is odd or even.
  - See answer [here](https://replit.com/@ZhangNing1/CSCI100NingZhang#EvenOddNumber.py)

## 3.3.10.3 nested-if
+ A nested if is an if statement that is the target of another if statement. Nested if statements mean an if statement inside another if statement. Yes, Python allows us to nest if statements within if statements. i.e, we can place an if statement inside another if statement.


<img src="https://media.geeksforgeeks.org/wp-content/cdn-uploads/20200710163548/Nested_if.jpg" alt="nested if statement" style="width:300px; height:400px">


+ Syntax
~~~~
if condition1:
   # Executes when condition1 is true
   if condition2: 
      # Executes when condition2 is true
   else:
      # Executes when condition2 is false
   # inner if-else ends here
else:
  # Executes when condition1 is false
  # you can also add if-else statements in this code block
# outter if-else ends here
~~~~

+ Example
~~~~
i = 20
if i>15:
  print("i is greater than 15")
  print("i'm in outter if Block")
  if i>30:
    print("i is greater than 30")
    print("i'm in inner if Block")
  else:
    print("i is smaller than 30")
    print("i'm in inner else Block")
else:
  print("i is smaller than or equal to 15")
  print("i'm in outter else Block")
~~~~


## 3.3.10.4 if-else-if statement
+ Here, a user can decide among multiple options. The if statements are executed from the top down. As soon as one of the conditions controlling the if is true, the statement associated with that if is executed, and the rest of the ladder is bypassed. If none of the conditions is true, then the final else statement will be executed.


<img src="https://media.geeksforgeeks.org/wp-content/uploads/if-elseif-ladder.jpg" alt=" if elif else statement" style="width:300px; height:400px">

+ Syntax
~~~~
if (condition):
    statement
elif (condition):
    statement
.
.
else:
    statement
~~~~

+ Example

~~~~
i = 20
if (i == 10):
    print("i is 10")
elif (i == 15):
    print("i is 15")
elif (i == 20):
    print("i is 20")
else:
    print("i is not present")
~~~~





