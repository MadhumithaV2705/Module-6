# Exp.No:28  
## Abstraction

---

### AIM 

To write a Python program to define an abstract base class named type_shape using the ABC module and declare an abstract method area().
---

### ALGORITHM

1. Start the program.
2. Import `ABC` and `abstractmethod` from the `abc` module.
3. Define an abstract base class `type_shape` with an abstract method `area()`.
4. Define the `Rectangle` class inheriting from `type_shape` and implement the `area()` method.
5. Define the `Circle` class inheriting from `type_shape` and implement the `area()` method.
6. Define the `Square` class inheriting from `type_shape` and implement the `area()` method.
7. Define the `triangle` class separately and implement the `area()` method.
8. Create objects for all classes and call the `area()` method.
9. Display the area of each shape.
10. End the program.


---

### PROGRAM

```
Reg.No: 212223060145
Name: Madhumitha V

from abc import ABC, abstractmethod
import math
class type_shape(ABC): 
    def area(self):
        pass

class Rectangle(type_shape):
  length = 6
  breadth = 4
  def area(self):
    return self.length * self.breadth

class Circle(type_shape):
  radius = 7
  def area(self):
      return 3.14*self.radius*self.radius

class Square(type_shape):
  length = 4
  def area(self):
      return 4*self.length
  

class triangle:
  length = 5
  width = 4
  def area(self):
      return 0.5*self.length*self.width
      
r = Rectangle() 
c = Circle() 
s = Square() 
t = triangle() 
print("Area of a rectangle:", r.area())
print("Area of a circle:", c.area()) 
print("Area of a square:", s.area()) 
print("Area of a triangle:", t.area()) 

```

### OUTPUT
<img width="644" height="224" alt="image" src="https://github.com/user-attachments/assets/eaa574b7-a846-4e7d-8162-82641da5b39a" />

### RESULT
Thus, the Python program to implement an abstract base class with an abstract method and calculate the areas of different shapes was successfully executed and verified.
