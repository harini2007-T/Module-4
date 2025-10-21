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
