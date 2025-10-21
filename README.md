# Classes and Objects in Python: Calculate the Area of a Circle

## 🎯 Aim
To write a Python program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `cse` and a method `mech` to perform the calculation.

## 🧠 Algorithm
1. **Get user input**: Take the radius of the circle as input from the user.
2. **Define the class**: Create a class named `cse`.
3. **Define the method**: Inside the class, define the method `mech` to calculate the area of the circle using the formula:  
   Area = pi *r^2 
4. **Execute the program**: Create an object of the class and call the method with the radius value.

## 🧾 Program
```
import math

class cse:
    def mech(self, radius):
        # Calculate the area of the circle
        area = math.pi * radius * radius
        return area
circle = cse()
r = float(input("Enter the radius of the circle: "))
area = circle.mech(r)
print("Area of the circle:", area)

```
## Output
<img width="454" height="67" alt="Screenshot 2025-10-14 212615" src="https://github.com/user-attachments/assets/363b5d33-4ea6-49b1-9cf8-fbabeda98624" />

## Result
The program successfully calculates the area of a circle using classes and objects
## Dictionary Operations in Python: Merging Two Dictionaries

## 🎯 Aim
To write a Python program that merges **two dictionaries** and combines their key-value pairs.

## 🧠 Algorithm
1. Define two dictionaries `dict1` and `dict2` with some key-value pairs.
2. Define a function `merge()` that merges the two dictionaries using the `**` unpacking operator.
   - The merged result will combine keys from both dictionaries. If a key exists in both, the value from `dict2` will overwrite that from `dict1`.
3. Call the `merge()` function and print the merged dictionary.

## 🧾 Program
Add code here
```
# Define two dictionaries
dict1 = {'a': 10, 'b': 20, 'c': 30}
dict2 = {'d': 40, 'b': 50, 'e': 60}

# Function to merge dictionaries
def merge(d1, d2):
    merged_dict = {**d1, **d2}  # Unpacking operator merges dictionaries
    return merged_dict

# Call the function and print the result
merged_result = merge(dict1, dict2)
print("Merged Dictionary:", merged_result)
```

## Output
<img width="802" height="48" alt="image" src="https://github.com/user-attachments/assets/75fb488e-fb17-42a8-9d79-8df56b84e49c" />


## Result
The program successfully merges two dictionaries.
All key-value pairs from both dictionaries are combined.
If a key exists in both dictionaries (like 'b'), the value from the second dictionary (dict2) overwrites the value from the first dictionary (dict1).

# 🔤 Dictionary-Python Program to Sort a Dictionary by Keys and Values

This Python program demonstrates how to sort a dictionary:
- Alphabetically by keys
- Alphabetically by values

---

## 🎯 Aim

To write a Python program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order

---

## 🧠 Algorithm

1. **Start the program.**
2. **Define** a dictionary with key-value pairs.
3. **Sort by Keys**:
   - Use `sorted(dictionary.items())`
   - Convert the result to a dictionary using `dict()`
4. **Sort by Values**:
   - Use `sorted(dictionary.items(), key=lambda item: item[1])`
   - Convert the result to a dictionary using `dict()`
5. **Display** the original and sorted dictionaries.
6. **End the program.**

---

## 🧪Program
```
my_dict = {
    'banana': 'yellow',
    'apple': 'green',
    'cherry': 'red',
    'date': 'brown'
}
sorted_by_keys = dict(sorted(my_dict.items()))
sorted_by_values = dict(sorted(my_dict.items(), key=lambda item: item[1]))

print("Dictionary sorted by keys:", sorted_by_keys)
print("Dictionary sorted by values:", sorted_by_values)
```

## Sample Output
<img width="809" height="106" alt="Screenshot 2025-10-14 213048" src="https://github.com/user-attachments/assets/593fdd52-08a9-4d26-8bdd-eb8361cf29ec" />

## Result
The program successfully sorts a dictionary

# Exception Handling in Python: Avoiding Index Errors

## 🎯 Aim
To write a Python program that handles an **IndexError** when trying to access an element beyond the available range of a list.

## 🧠 Algorithm
1. Define a list `list1` with some integer elements.
2. Use a **try-except** block:
   - In the `try` block, attempt to access an index that is out of range (e.g., `list1[5]`).
   - In the `except` block, catch the error and print a custom message `"You're out of list range"`.
3. Print the result based on whether the index access succeeds or fails.

## 🧾 Program
Add code here
```
# Define a list
list1 = [10, 20, 30, 40]

# Try to access an element out of range
try:
    print(list1[5])
except IndexError:
    print("You're out of list range")
```


## Output
<img width="836" height="75" alt="image" src="https://github.com/user-attachments/assets/73f91f7f-7926-4cd7-8cb4-d070a41e6aaf" />



## Result
The program successfully handles an IndexError when attempting to access a list element beyond its range.
Instead of crashing, it prints a custom message, informing the user that the requested index is out of range.

# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program
```
import csv
count = 0
with open('story.txt', 'r') as file:
    for line in file:
        stripped_line = line.lstrip()
        if stripped_line and not stripped_line.startswith('T'):
            count += 1
print("Number of lines not starting with 'T':", count)
```
## Output
<img width="423" height="46" alt="Screenshot 2025-10-14 214622" src="https://github.com/user-attachments/assets/e152cf7a-8000-4fcb-b3bc-6fdd803780f8" />

## Result
The program successfully counts the number of lines in text file
