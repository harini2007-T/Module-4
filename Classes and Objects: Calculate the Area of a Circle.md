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
