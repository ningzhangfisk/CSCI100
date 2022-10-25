# Python Datastructures
+ Lists
+ Tuples
+ Set
+ Dictionaries

# 1. Lists
+ Lists are used to store multiple items in a single variable.

## 1.1 Create a list
+ Lists are created using square brackets:

~~~~
thislist = ["apple", "banana", "cherry"]
print(thislist)
~~~~

## 1.2 Access Items
+ List items are indexed and you can access them by referring to the index number:

~~~~
thislist = ["apple", "banana", "cherry"]
print(thislist[1])
~~~~

+ Negative Indexing: Negative indexing means start from the end. `-1` refers to the last item, `-2` refers to the second last item etc.

~~~~
thislist = ["apple", "banana", "cherry"]
print(thislist[-1])
~~~~


+ Check if Item Exists: To determine if a specified item is present in a list use the `in` keyword:

~~~~
thislist = ["apple", "banana", "cherry"]
if "apple" in thislist:
  print("Yes, 'apple' is in the fruits list")
~~~~

## 1.3 Change Item Value
+ To change the value of a specific item, refer to the index number:
~~~~
# Change the second item:
thislist = ["apple", "banana", "cherry"]
thislist[1] = "blackcurrant"
print(thislist)
~~~~

## 1.4 Insert Items: 
+ To insert a new list item, without replacing any of the existing values, we can use the `insert()` method.
+ The insert() method inserts an item at the specified index:

~~~~
# Insert "watermelon" as the third item:
thislist = ["apple", "banana", "cherry"]
thislist.insert(2, "watermelon")
print(thislist)
~~~~

## 1.5 Append Items
+ To add an item to the end of the list, use the `append()` method:

~~~~
thislist = ["apple", "banana", "cherry"]
thislist.append("orange")
print(thislist)
~~~~

## 1.6 Remove Specified Item or Index
+ The `remove()` method removes the specified item.

~~~~
# Remove "banana":
thislist = ["apple", "banana", "cherry"]
thislist.remove("banana")
print(thislist) 
~~~~

+ `The pop()` method removes the specified index. If you do not specify the index, the pop() method removes the last item.

~~~~
# Remove the second item:
thislist = ["apple", "banana", "cherry"]
thislist.pop(1)
print(thislist)


# Remove the last item:
thislist = ["apple", "banana", "cherry"]
thislist.pop()
print(thislist)
~~~~

## 1.7 Loop Lists
+ Loop Through a List: You can loop through the list items by using a for loop:

~~~~
# Print all items in the list, one by one:
thislist = ["apple", "banana", "cherry"]
for x in thislist:
  print(x)
~~~~

+ Loop Through the Index Numbers: Use the range() and len() functions to create a suitable iterable.

~~~~
# Print all items by referring to their index number:
thislist = ["apple", "banana", "cherry"]
for i in range(len(thislist)):
  print(thislist[i])
~~~~

## 1.8 Sort Lists
+  Sort List Alphanumerically:  List objects have a `sort()` method that will sort the list alphanumerically, ascending, by default:

~~~~
# Sort the list alphabetically:
thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]
thislist.sort()
print(thislist)

# Sort the list numerically:
thislist = [100, 50, 65, 82, 23]
thislist.sort()
print(thislist)
~~~~

+ To sort descending, use the keyword argument `reverse = True`:

~~~~
# Sort the list descending:
thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]
thislist.sort(reverse = True)
print(thislist)


thislist = [100, 50, 65, 82, 23]
thislist.sort(reverse = True)
print(thislist)
~~~~

## 1.9 Join Two Lists
+ There are several ways to join, or concatenate, two or more lists in Python.
+ One of the easiest ways are by using the `+` operator.

~~~~
# Join two list:
list1 = ["a", "b", "c"]
list2 = [1, 2, 3]

list3 = list1 + list2
print(list3)
~~~~
