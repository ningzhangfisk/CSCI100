# 3. Sets
+ Sets are used to store multiple items in a single variable.
+ Set is one of 4 built-in data types in Python used to store collections of data, the other 3 are List, Tuple, and Dictionary, all with different qualities and usage.
+ A set is a collection which is `unordered`, `unchangeable`, and `unindexed`.
  - Set items are unchangeable, but you can remove items and add new items.

## 3.1 Create a Set
+ Sets are written with curly brackets.
~~~~
thisset = {"apple", "banana", "cherry"}
print(thisset)
~~~~
+ Duplicates Not Allowed
+ Duplicate values will be ignored.
~~~~
thisset = {"apple", "banana", "cherry", "apple"}
print(thisset)
~~~~
+ Get the Length of a Set

~~~~
thisset = {"apple", "banana", "cherry"}
print(len(thisset))
~~~~
## 3.2 Access Items
+ You cannot access items in a set by referring to an index or a key.
+ But you can loop through the set items using a `for` loop, or ask if a specified value is present in a set, by using the `in` keyword.


~~~~
# Loop through the set, and print the values:
thisset = {"apple", "banana", "cherry"}
for x in thisset:
  print(x)
  
# Check if "banana" is present in the set:  
thisset = {"apple", "banana", "cherry"}
print("banana" in thisset)
~~~~

## 3.3 Add Items
+ Once a set is created, you cannot change its items, but you can add new items.
+ Add an item to a set, using the `add()` method
~~~~
thisset = {"apple", "banana", "cherry"}
thisset.add("orange")
print(thisset)
~~~~

## 3.4 Add Sets
+ To add items from another set into the current set, use the `update()` method.

~~~~
thisset = {"apple", "banana", "cherry"}
tropical = {"pineapple", "mango", "papaya"}
thisset.update(tropical)
print(thisset)
~~~~

## 3.5 Remove Item
+ To remove an item in a set, use the `remove()`, or the `discard()` method.

~~~~
# Remove "banana" by using the remove() method:
thisset = {"apple", "banana", "cherry"}
thisset.remove("banana")
print(thisset)

# Remove "banana" by using the discard() method:
thisset = {"apple", "banana", "cherry"}
thisset.discard("banana")
print(thisset)
~~~~

+ You can also use the `pop()` method to remove an item, but this method will remove the last item. Remember that sets are unordered, so you will not know what item that gets removed.

~~~~
thisset = {"apple", "banana", "cherry"}
x = thisset.pop()
print(x)
print(thisset)
~~~~

+ The `clear()` method empties the set
~~~~
thisset = {"apple", "banana", "cherry"}
thisset.clear()
print(thisset)
~~~~

+ The `del` keyword will delete the set completely

~~~~
thisset = {"apple", "banana", "cherry"}
del thisset
print(thisset)
~~~~
## 3.6 Loop Items
+ You can loop through the set items by using a for loop:

~~~~
thisset = {"apple", "banana", "cherry"}

for x in thisset:
  print(x)
~~~~

## 3.7 Join Two Sets
+ You can use the `union()` method that returns a new set containing all items from both sets,
+  or the `update()` method that inserts all the items from one set into another

~~~~
# The union() method returns a new set with all items from both sets:
set1 = {"a", "b" , "c"}
set2 = {1, 2, 3}

set3 = set1.union(set2)
print(set3)

# The update() method inserts the items in set2 into set1:
set1 = {"a", "b" , "c"}
set2 = {1, 2, 3}

set1.update(set2)
print(set1)
~~~~

## 3.8 Set Methods
+ See method descriptions [here](https://www.w3schools.com/python/python_sets_methods.asp)

