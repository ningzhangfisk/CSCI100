## 3.3.8 Logical Operators
### Questions: True or False
+ Are your favorite activities hiking `AND` traveling?
+ Have you had coffee `OR` tea this morning?
+ Are you `NOT` excited for the weekend?
+ Do we have Monday `AND` `NOT` Tuesday off for Labor Day?

### 3.3.8.1 What are Logical Operators?
+ Reminder: Arithmetic operators (`+`, `-`, `*`, `/`) to combine numbers
+ Logical operators: combine booleans
  - `and`
  - `or`
  - `not`
#### Logical Operators: `AND`
+ `AND` returns true only if both operands are true.

![and_operator](../Resources/and_operator.png)

+ Practice: Milkshake Time!
~~~~
vanilla = True
chocolate = True
strawberry = False


vanilla and strawberry
vanilla and chocolate
chocolate and vanilla
chocolate and strawberry
strawberry and strawberry
~~~~

<details>
    <summary>Click to see the answer!</summary>
    vanilla and strawberry    ->   False<br>
    vanilla and chocolate     ->   True<br>
    chocolate and vanilla     ->   True<br>
    chocolate and strawberry  ->   False<br>
    strawberry and strawberry ->   False
</details>


#### Logical Operators: `OR`
+ `OR` returns true if either (or both) operand is true.

![or orperator](../Resources/or_operator.png)

+ Practice: Outdoor Activities!
~~~~
hiking = True
running = False
biking = False


hiking or running
hiking or biking
biking or hiking
biking or running
running or biking
~~~~

<details>
    <summary>Click to see the answer!</summary>
    hiking or running  ->     True<br>
    hiking or biking   ->     True<br>
    biking or hiking   ->     True<br>
    biking or running  ->     False<br>
    running or biking  ->     False
</details>



#### Logical Operators: `NOT`
+ `NOT` inverts (gives opposite value of) the value of its operand.

![not orperator](../Resources/not_operator.png)

+ Practice: Favorite Colors!
~~~~
blue = True
red = False
green = True

not blue
not red
not green
~~~~

<details>
    <summary>Click to see the answer!</summary>
    not blue  ->   False  <br>
    not red   ->   True   <br>
    not green ->   False  <br>
</details>

#### How is `not` different from `and` and `or`?

![logic comparison](../Resources/logic_comparison.png)


#### Combining Operators

![combine operators](../Resources/combine_operators.png)

+ Practice 1:
~~~~
True and not False
(False or True) and False
not (True or False) or True
~~~~

<details>
    <summary>Click to see the answer!</summary>
    True and not False           ->       True<br>
    (False or True) and False    ->       False<br>
    not (True or False) or True  ->       True
</details>

+ Practice 2:  Animals on a Farm!
~~~~
dog = False
chicken = True
sheep = True

not dog or not chicken and sheep
chicken and dog or not sheep
not chicken or not sheep or dog
dog and not sheep or chicken 
~~~~

<details>
    <summary>Click to see the answer!</summary>
    not dog or not chicken and sheep   ->   True<br>
    chicken and dog or not sheep       ->   False <br>
    not chicken or not sheep or dog    ->   False<br>
    dog and not sheep or chicken       ->   True
</details>

+ Practice 3: Find the bug in the following code.
~~~~
answer = input("What city is Fisk in?")
if answer == "nashville" or "Nashville":
  print("Correct!")
~~~~

<details>
    <summary>Click to see the explanation!</summary>

![nashville 1](../Resources/nashville1.png)
  
![nashville 2](../Resources/nashville2.png)
  
![nashville 3](../Resources/nashville3.png)
  
![nashville 4](../Resources/nashville4.png)
</details>




<details>
    <summary>Click to see the correct code!</summary>
    answer = input("What city is Fisk in?")
    if answer == "nashville" or answer == "Nashville":
      print("Correct!")
</details>
