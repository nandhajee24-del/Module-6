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
