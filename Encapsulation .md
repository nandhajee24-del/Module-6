# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
```py
# Step 1: Define the Class
class Rectangle:
    def __init__(self, length, breadth):
        # Step 2: Initialize Variables
        self.__length = length
        self.__breadth = breadth

    def display(self):
        # Step 3: Print Values
        print("Length:", self.__length)
        print("Breadth:", self.__breadth)

# Step 4: Instantiate the Object
rect = Rectangle(10, 5)
rect.display()
```
## Output
<img width="199" height="68" alt="Screenshot 2025-10-22 225736" src="https://github.com/user-attachments/assets/6abe8a86-219b-44ea-a693-b37bf14cf9ff" />

## Result
successfully **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.
 
