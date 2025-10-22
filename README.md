A.Nandha(25017364)
# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
```py
# Step 1: Import ABC module
from abc import ABC, abstractmethod
import math

# Step 2: Create Abstract Class
class Shape(ABC):
    @abstractmethod
    def calculate_area(self):
        pass

# Step 3: Create Subclass Rectangle
class Rectangle(Shape):
    def __init__(self, length=5, breadth=3):
        self.length = length
        self.breadth = breadth

    def calculate_area(self):
        return self.length * self.breadth

# Step 4: Create Subclass Circle
class Circle(Shape):
    def __init__(self, radius=4):
        self.radius = radius

    def calculate_area(self):
        return math.pi * self.radius ** 2

# Step 5: Create Objects & Call Methods
rect = Rectangle()
circle = Circle()

print("Rectangle Area:", rect.calculate_area())
print("Circle Area:", round(circle.calculate_area(), 2))
```
## Output
<img width="303" height="96" alt="Screenshot 2025-10-22 225510" src="https://github.com/user-attachments/assets/b1ba0ac4-3924-4113-84b6-db1f270ca8b4" />

## Result
successfully **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.


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
 

 # 🐟 Method Overriding-Fish and Shark Class Inheritance in Python

## 🧠 AIM:
To write a Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method.

## 📋 ALGORITHM:

1. Define the `Fish` class with a method named `type()` that prints `"fish"`.
2. Define the `Shark` class as a subclass of `Fish`, and override the `type()` method to print `"shark"`.
3. Create an instance of the `Fish` class named `obj_goldfish`.
4. Create an instance of the `Shark` class named `obj_hammerhead`.
5. Use a `for` loop to iterate over both objects.
6. Within the loop, call the `type()` method using the loop variable.
7. Output will demonstrate method overriding: printing `"fish"` and `"shark"` accordingly.

## 💻 PROGRAM:
```py
# Step 1: Define the Fish class
class Fish:
    def type(self):
        print("fish")

# Step 2: Define the Shark class as a subclass of Fish
class Shark(Fish):
    def type(self):
        print("shark")

# Step 3 & 4: Create instances
obj_goldfish = Fish()
obj_hammerhead = Shark()

# Step 5 & 6: Iterate and call type() method
for fish in [obj_goldfish, obj_hammerhead]:
    fish.type()
```
## OUTPUT
<img width="132" height="77" alt="Screenshot 2025-10-22 225942" src="https://github.com/user-attachments/assets/cf7def75-d3a9-4c07-a0d8-d30b82d2013c" />

## RESULT
successfully Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method.

# 🐍 Python OOP: Operator Overloading (Less Than `<`)

## 🎯 AIM

To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.

---

## 🧠 ALGORITHM

1. **Create Class `A`**:
   - Define the `__init__()` method to initialize the object with a value `a`.

2. **Overload the `<` Operator**:
   - Define the `__lt__()` method with logic:
     - If `self.a < o.a`, return `"ob1 is less than ob2"`
     - Else, return `"ob2 is less than ob1"`

3. **Create Objects**:
   - Instantiate two objects `ob1` and `ob2` with values.

4. **Use `<` Operator**:
   - Use `print(ob1 < ob2)` to trigger the overloaded behavior.

---

## 💻 Program
```py
# Step 1: Create Class A
class A:
    def __init__(self, a):
        self.a = a

    # Step 2: Overload the < operator
    def __lt__(self, o):
        if self.a < o.a:
            return "ob1 is less than ob2"
        else:
            return "ob2 is less than ob1"

# Step 3: Create Objects
ob1 = A(10)
ob2 = A(20)

# Step 4: Use < Operator
print(ob1 < ob2)
```
## Output
<img width="393" height="72" alt="Screenshot 2025-10-22 230200" src="https://github.com/user-attachments/assets/2210d961-d7ff-4b3b-975a-a06fc7066373" />

## Result
successfully Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.


# # 🐍 Python OOP: Polymorphism with Classes

## 🎯 AIM

To create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.

---

## 🧠 ALGORITHM

1. **Create Class `Beans`**:
   - Define `type()` method that prints `"Vegetable"`.
   - Define `color()` method that prints `"Green"`.

2. **Create Class `Mango`**:
   - Define `type()` method that prints `"Fruit"`.
   - Define `color()` method that prints `"Yellow"`.

3. **Define Generic Function `func(obj)`**:
   - Call `obj.type()` and `obj.color()` — this works with both `Beans` and `Mango` objects, showcasing **polymorphism**.

4. **Create Objects**:
   - Instantiate `Beans` and `Mango`.
   - Pass them to `func()` and execute the program.

---

## 💻 Program
```py
# Step 1: Create Class Beans
class Beans:
    def type(self):
        print("Vegetable")
    
    def color(self):
        print("Green")

# Step 2: Create Class Mango
class Mango:
    def type(self):
        print("Fruit")
    
    def color(self):
        print("Yellow")

# Step 3: Define Generic Function
def func(obj):
    obj.type()
    obj.color()

# Step 4: Create Objects and Call Function
b = Beans()
m = Mango()

func(b)
func(m)
```
## Output
<img width="207" height="158" alt="Screenshot 2025-10-22 230350" src="https://github.com/user-attachments/assets/51a5335c-79f8-4fd9-b38b-f9e57ca79d28" />

## Result
successfully **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.

