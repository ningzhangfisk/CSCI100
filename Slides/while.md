# 3.3.11 While Loop

+ A `while` loop statement in Python programming language repeatedly executes a target statement as long as a given condition is true.

![python_while_loop ](https://www.tutorialspoint.com/python/images/python_while_loop.jpg)

## 3.3.11.1 Syntax
+ The `statement(s)` may be a single statement or a block of statements. 
+ The `condition` may be any expression, and true is any non-zero value. 
+ The loop iterates while the `condition` is true.
+ When the condition becomes false, program control passes to the line immediately following the loop.
+ Here, key point of the while loop is that the loop might not ever run. When the condition is tested and the result is false, the loop body will be skipped and the first statement after the while loop will be executed.

~~~~~
while condition:
   statement(s)
~~~~~

+ Example: The block here, consisting of the print and increment statements, is executed repeatedly until count is no longer less than 9. With each iteration, the current value of the index count is displayed and then increased by 1.

~~~~
count = 0
while (count < 9):
  print('The count is:', count)
  count = count + 1

print("Good bye!")
~~~~

+ Note a `while` loop can be converted to a `for` loop, or vice versa.
~~~~
for count in range(9):
  print('The count is:', count)

print("Good bye!")
~~~~

## 3.3.11.2 The Infinite Loop
+ A loop becomes infinite loop if a condition never becomes `False`. You must use caution when using while loops because of the possibility that this condition never resolves to a `False` value. This results in a loop that never ends. Such a loop is called an infinite loop.
+ An infinite loop might be useful in client/server programming where the server needs to run continuously so that client programs can communicate with it as and when required.
+ Example
~~~~
var = 1
while var == 1 :  # This constructs an infinite loop
  num = input("Enter a number: ")
  print("You entered: ", num)

print("Good bye!")
~~~~
+ To terminate an infinite loop, you can either click the `Stop` button(the `Run` button turns into `Stop` when having an infinite loop) or use `control + c`(press `control` and `c` keys at the same time)
## 3.3.11.3 Using else Statement with While Loop
+ If the `else` statement is used with a `while` loop, the else statement is executed when the condition becomes `False`.
+ Example: The following example illustrates the combination of an else statement with a while statement that prints a number as long as it is less than 5, otherwise else statement gets executed
~~~~
count = 0
while count < 5:
  print(count, "is less than 5")
  count = count + 1
else:
  print(count, "is not less than 5")
~~~~

## 3.3.11.4 The break Statement
+ With the `break` statement we can stop the loop even if the while condition is true.
+ Example 1:
~~~~
i = 1
while i < 6:
  print(i)
  if i == 3:
    break
  i += 1
~~~~
+ Example 2:
~~~~
answer = 4
var = 1
while var == 1:  # This constructs an infinite loop
  num = int(input("Enter a number to have a guess: "))
  print("You entered: ", num)
  if num == answer:
    print("Your answer is correct.")
    break
  else:
    print("Your answer is Not correct.")

print("Good bye!")
~~~~

## 3.3.11.5 The continue Statement
+ With the `continue` statement we can stop the current iteration, and continue with the next.
+ Example: Continue to the next iteration if i is 3.
~~~~
i = 0
while i < 6:
  i += 1
  if i == 3:
    continue
  print(i)
~~~~
# Reference
[tutorialspoint](https://www.tutorialspoint.com/python/python_while_loop.htm)
