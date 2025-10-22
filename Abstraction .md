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
