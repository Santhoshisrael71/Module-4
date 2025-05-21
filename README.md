# Ex 4.1: Classes and Objects in Python: Calculate the Area of a Circle

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
        area = math.pi * radius ** 2
        print(f"Area of circle: {area:.2f}")
r = float(input())
obj = cse()
obj.mech(r)
````
## Output

![image](https://github.com/user-attachments/assets/993609a9-e6a8-4263-9f4f-d284b5d261c7)


## Result

Python program executed successfully.


# Ex 4.2: Dictionary Operations in Python: Merging Two Dictionaries

## 🎯 Aim
To write a Python program that merges **two dictionaries** and combines their key-value pairs.

## 🧠 Algorithm
1. Define two dictionaries `dict1` and `dict2` with some key-value pairs.
2. Define a function `merge()` that merges the two dictionaries using the `**` unpacking operator.
   - The merged result will combine keys from both dictionaries. If a key exists in both, the value from `dict2` will overwrite that from `dict1`.
3. Call the `merge()` function and print the merged dictionary.

## 🧾 Program
```
a=eval(input())
b=eval(input())
c=a.copy()
c.update(b)
print(c)
```
## Output

![image](https://github.com/user-attachments/assets/3952f34c-adc1-4232-9364-d4439948593f)


## Result

Python program executed successfully.




# Ex 4.3:  Dictionary-Python Program to Sort a Dictionary by Keys and Values

This Python program demonstrates how to sort a dictionary:
- Alphabetically by keys
- Alphabetically by values


## 🎯 Aim

To write a Python program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order



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



## 🧪Program
```
input_dict = {2: 56, 1: 2, 5: 12, 4: 24, 6: 18, 3: 323}
sorted_items = sorted(input_dict.items())
print("Keys and Values sorted in alphabetical order by the key")
for key, value in sorted_items:
    print(f"({key}, {value})", end=' ')
```
##  Output

![image](https://github.com/user-attachments/assets/0c4863cf-0ebd-41d0-8b1e-7393ed514e72)


## Result

Python program executed successfully.



# Ex 4.4: Exception Handling in Python: Avoiding Index Errors

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
try:
    # Taking 3 elements input from the user
    L = []
    for i in range(3):
        item = ['laptop','mobile','pen']
        L.append(item)

    # Trying to access index 4
    print(L[4])

except IndexError:
    print("check index range")
```
## Output

![image](https://github.com/user-attachments/assets/6d327293-eb33-416d-8531-144c5375c6a4)


## Result
Python program executed successfully.




# Ex 4.5: File Handling in Python: Count Lines Not Starting with 'T'

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
        if line.strip() and not line.lstrip().startswith('T'):
            count += 1
print("Sum :", count)
```

## Output
![image](https://github.com/user-attachments/assets/e89d4e50-2ae4-41e6-a76f-a7181ecc55a6)

## Result
Python program executed successfully.
