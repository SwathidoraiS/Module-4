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
    def mech(self, r):
        area = math.pi * r ** 2
        print(f"The area of the circle is: {area}")

radius = float(input("Enter the radius of the circle: "))
circle = cse()
circle.mech(radius)
```

## Output
![image](https://github.com/user-attachments/assets/2243be82-07ec-41a2-b592-f8f58e19e18e)


## Result
Thus the program is sucessfully executed.

## Dictionary Operations in Python: Merging Two Dictionaries

## 🎯 Aim
To write a Python program that merges **two dictionaries** and combines their key-value pairs.

## 🧠 Algorithm
1. Define two dictionaries `dict1` and `dict2` with some key-value pairs.
2. Define a function `merge()` that merges the two dictionaries using the `**` unpacking operator.
   - The merged result will combine keys from both dictionaries. If a key exists in both, the value from `dict2` will overwrite that from `dict1`.
3. Call the `merge()` function and print the merged dictionary.

## 🧾 Program
```
def merge(dict1, dict2):
    merged_dict = {**dict1, **dict2}
    print(merged_dict)

dict1 = {'a': 1, 'b': 2, 'c': 3}
dict2 = {'b': 4, 'd': 5}

merge(dict1, dict2)
```
## Output
![image](https://github.com/user-attachments/assets/71a8932f-f4ba-4119-9510-502f814d9ffc)


## Result
Thus the program is sucessfully executed.

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
# Start the program
dictionary = {'apple': 3, 'banana': 1, 'cherry': 2, 'date': 4}

# Sort by Keys
sorted_by_keys = dict(sorted(dictionary.items()))

# Sort by Values
sorted_by_values = dict(sorted(dictionary.items(), key=lambda item: item[1]))

# Display the original and sorted dictionaries
print("Original Dictionary:", dictionary)
print("Sorted by Keys:", sorted_by_keys)
print("Sorted by Values:", sorted_by_values)
```

## Sample Output
![image](https://github.com/user-attachments/assets/34549491-b12f-4a5d-a35b-26ba3583824c)


## Result
Thus the program is sucessfully executed.

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
```
list1 = [1, 2, 3, 4]

try:
    print(list1[5])
except IndexError:
    print("You're out of list range")
```
## Output
![image](https://github.com/user-attachments/assets/116fffc2-7b9c-4470-b9f2-8d0bb5c772fb)


## Result
Thus the program is sucessfully executed.

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
count = 0

with open("story.txt", "r") as file:
    for line in file:
        if not line.startswith('T'):
            count += 1

print(count)
```

## Output
![image](https://github.com/user-attachments/assets/c51a323e-ca8c-48be-84a2-578842647d86)


## Result
Thus the program is sucessfully executed.
