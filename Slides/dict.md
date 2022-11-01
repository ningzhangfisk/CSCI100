# 4. Dictionaries
+ Dictionaries are used to store data values in `key:value` pairs.
+ A dictionary is a collection which is `ordered`, `changeable` and do not allow duplicates.


## 4.1 Create a dictionary
+ Dictionaries are written with curly brackets, and have keys and values

~~~
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict)
~~~


## 4.2 Accessing Items
+ You can access the items of a dictionary by referring to its key name, inside square brackets:

~~~~
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
x = thisdict["model"]
~~~~


+ There is also a method called get() that will give you the same result:

~~~~
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
x = thisdict.get("model")
~~~~

## 4.3 Check if Key Exists
+ To determine if a specified key is present in a dictionary use the `in` keyword:

~~~
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
if "model" in thisdict:
  print("Yes, 'model' is one of the keys in the thisdict dictionary")
~~~

## 4.4 Change Values
+ You can change the value of a specific item by referring to its key name:


~~~~
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict["year"] = 2018
~~~~

+ Update Dictionary

~~~~
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.update({"year": 2020})
~~~~

## 4.5 Adding Items

+ Adding an item to the dictionary is done by using a new index key and assigning a value to it:


~~~~
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict["color"] = "red"
print(thisdict)
~~~~

## 4.6 Removing Items
+ The `pop()` method removes the item with the specified key name:

~~~~
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.pop("model")
print(thisdict)
~~~~

+ The `popitem()` method removes the last inserted item:

~~~~
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.popitem()
print(thisdict)
~~~~

+ The `del` keyword removes the item with the specified key name:

~~~~
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
del thisdict["model"]
print(thisdict)
~~~~

+ The `del` keyword can also delete the dictionary completely:

~~~~
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
del thisdict
print(thisdict) #this will cause an error because "thisdict" no longer exists.
~~~~

+ The `clear()` method empties the dictionary:

~~~~
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.clear()
print(thisdict)
~~~~

# 4.7 Loop Through a Dictionary

+ You can loop through a dictionary by using a `for` loop.

~~~~
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}

# Print all key names in the dictionary, one by one:
for x in thisdict:
  print(x)
# You can use the keys() method to return the keys of a dictionary:
for x in thisdict.keys():
  print(x)
  
# Print all values in the dictionary, one by one:
for x in thisdict:
  print(thisdict[x])
# You can also use the values() method to return values of a dictionary:
for x in thisdict.values():
  print(x)


# Loop through both keys and values, by using the items() method:
for x, y in thisdict.items():
  print(x, y)
~~~~

## 4.8  Dictionary Methods

See dictionary methods [here](https://www.w3schools.com/python/python_dictionaries_methods.asp)
