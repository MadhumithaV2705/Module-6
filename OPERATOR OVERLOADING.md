# Exp.No:27  
## Operator Overloading

---

### AIM  
To write a Python program to overload the division operator (/) in a user-defined complex class to perform division between two complex number objects and display the result.

---

### ALGORITHM

1. Start the program.
2. Define a class `complex` to represent complex numbers.
3. Create a constructor `__init__()` to initialize the real part `a` and imaginary part `b`.
4. Overload the division operator `__truediv__()` to divide the corresponding real and imaginary parts of two complex numbers.
5. Overload the `__str__()` method to return the complex number in a readable format.
6. Create two objects `Ob1` and `Ob2` of the `complex` class with initial values.
7. Divide `Ob1` by `Ob2` using the overloaded division operator and store the result in `Ob3`.
8. Print the result `Ob3`.
9. End the program.


---

### PROGRAM

```
Reg.No: 212223060145
Name: Madhumitha V

class complex:
    def __init__(self, a, b):
        self.a = a
        self.b = b

    def __truediv__(self, other):
        real=self.a/other.a
        imag=self.b/other.b
        return complex(real, imag)
    def __str__(self):
        return f"({self.a}, {self.b})"
Ob1 = complex(10, 21)
Ob2 = complex(2, 3)
Ob3 = Ob1 / Ob2
print(Ob3)
```

### OUTPUT
<img width="487" height="155" alt="image" src="https://github.com/user-attachments/assets/cf8145d8-9c12-4cb1-a8aa-c740888ff80f" />

### RESULT
Thus, the program to overload the division operator for complex numbers was executed successfully and the output was verified.
