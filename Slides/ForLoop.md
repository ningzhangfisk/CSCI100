# 3.3.9 For Loops

## 3.3.9.1 Introduction
+ `for loop`: control structure that runs block of code repeatedly by iterating over elements in sequence

~~~
for letter in 'cat':
  print(letter)
  
print("done")
~~~

+ Tracing for loops

![for1](../Resources/for1.png)

![for2](../Resources/for2.png)

![for3](../Resources/for3.png)

![for4](../Resources/for4.png)

![for5](../Resources/for5.png)

![for6](../Resources/for6.png)

![for7](../Resources/for7.png)

![for8](../Resources/for8.png)


+ Accumulator Pattern

~~~~
word = 'friends'
result = ''
for char in word:
  result = result + char + '-'
print(result) # the result is f-r-i-e-n-d-s-
~~~~

+ `in` operator
  - `in` operator: checks if value exists in sequence
  - `in` expression evaluates to True if value exists

~~~~~
word = 'banana'
if 'n' in word:
  print('Found an n')
else:
  print('Did not find a n')
~~~~~

+ Practice: in operator
~~~~
'N' in 'Nashville, TN'<br>
'n' in 'Nashville, TN''<br>


char = ' '
char in 'Intro to Computer Science'


word = 'CS110'
char in word
~~~~

<details>
    <summary>Click to see the explanation!</summary>

![inpractice 1](../Resources/in_practice.png)
</details>

# Summary
+ What is an `in for loop`?
  - Control structure that runs block of code repeatedly by iterating over elements in sequence
  - Syntax
  ~~~~
  for [variable] in [sequence]:
    [execute code]
  ~~~~

+ Why is it important?
  - Write code once and run many times - do not need to copy and paste same code over and over

