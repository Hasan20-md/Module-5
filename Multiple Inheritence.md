# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
```
# Step 1: Calculation1 class
class Calculation1:
    def Summation(self, a, b):
        return a + b


# Step 2: Calculation2 class
class Calculation2:
    def Subtraction(self, a, b):
        return a - b


# Step 3: Derived class (Multiple Inheritance)
class Derived(Calculation1, Calculation2):
    def Division(self, a, b):
        if b != 0:
            return a / b
        else:
            return "Division by zero not allowed"


# Step 4: Input
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

# Step 5: Process
obj = Derived()
sum_result = obj.Summation(a, b)
sub_result = obj.Subtraction(a, b)
div_result = obj.Division(a, b)

# Step 6: Output
print("\nResults:")
print("Sum:", sum_result)
print("Difference:", sub_result)
print("Division:", div_result)
```
## Output Example
<img width="398" height="335" alt="image" src="https://github.com/user-attachments/assets/bf0bad37-bc7b-449a-8d11-00f8fbaeefff" />

## Result:
Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.
