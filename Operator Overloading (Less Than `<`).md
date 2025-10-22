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
