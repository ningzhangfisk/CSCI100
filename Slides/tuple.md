# 2. Tuples

+ Tuples are used to store multiple items in a single variable.
+ Tuple is one of 4 built-in data types in Python used to store collections of data, the other 3 are List, Set, and Dictionary, all with different qualities and usage.
+ A tuple is a collection which is ordered and unchangeable.
  - Tuples are unchangeable, meaning that we cannot change, add or remove items after the tuple has been created.
+ Tuples are written with round brackets.

## 2.1 Create a Tuple

~~~~
# create a tuple
thistuple = ("apple", "banana", "cherry")
print(thistuple)

# Tuples allow duplicate values:
thistuple = ("apple", "banana", "cherry", "apple", "cherry")
print(thistuple)

# Tuple Length
thistuple = ("apple", "banana", "cherry")
print(len(thistuple))

# Create Tuple With One Item
thistuple = ("apple",)
print(type(thistuple))
#NOT a tuple
thistuple = ("apple")
print(type(thistuple))
~~~~

## 2.2 Access Tuple Items
+ You can access tuple items by referring to the index number, inside square brackets:
~~~~
# Print the second item in the tuple:
thistuple = ("apple", "banana", "cherry")
print(thistuple[1])
# Negative Indexing
print(thistuple[-1])
# Check if Item Exists
thistuple = ("apple", "banana", "cherry")
if "apple" in thistuple:
  print("Yes, 'apple' is in the fruits tuple")
~~~~


## 2.3 Unpacking a Tuple
+ When we create a tuple, we normally assign values to it. This is called "packing" a tuple:

~~~~
fruits = ("apple", "banana", "cherry")
~~~~
+ But, in Python, we are also allowed to extract the values back into variables. This is called "unpacking":

~~~~
fruits = ("apple", "banana", "cherry")

(green, yellow, red) = fruits

print(green)
print(yellow)
print(red)
~~~~

## 2.4 Loop Through a Tuple
+ You can loop through the tuple items by using a for loop.

~~~~
thistuple = ("apple", "banana", "cherry")
for x in thistuple:
  print(x)
~~~~

or using `range` function

~~~~
thistuple = ("apple", "banana", "cherry")
for i in range(len(thistuple)):
  print(thistuple[i])
~~~~

or using `while` loop
~~~~
thistuple = ("apple", "banana", "cherry")
i = 0
while i < len(thistuple):
  print(thistuple[i])
  i = i + 1
~~~~

## 2.5 Join Two Tuples

~~~~
tuple1 = ("a", "b" , "c")
tuple2 = (1, 2, 3)

tuple3 = tuple1 + tuple2
print(tuple3)
~~~~

## 2.6 Tuple Methods
+ Python has two built-in methods that you can use on tuples.
  - `count()`:	Returns the number of times a specified value occurs in a tuple
  - `index()`:	Searches the tuple for a specified value and returns the position of where it was found


~~~~
thistuple = (1,2,3,4,5,1)
print(thistuple.count(1))
print(thistuple.index(1))
~~~~
