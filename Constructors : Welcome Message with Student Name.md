# # Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.

## 🧠 Algorithm
1. **Get user input**: Accept the student's name from the user.
2. **Define the class**: Create a class `Student` with a default constructor (`__init__`).
3. **Default Constructor**: In the constructor, assign the user input (student name) to an instance variable `self.a`.
4. **Display Message**: Define a method `show` that prints "This is non-parameterized constructor" and a welcome message with the student’s name.
5. **Execute the Program**: Instantiate the `Student` class and call the `show` method.

## 🧾 Program
```
name = input("Enter student name: ")

class Student:
    
    def __init__(self):
        self.a = name
    
    def show(self):
        print("This is non-parameterized constructor")
        print("Welcome", self.a)

obj = Student()
obj.show()
```

## Output
<img width="542" height="219" alt="image" src="https://github.com/user-attachments/assets/df1c40e2-3fbc-42f3-96af-df40043578f4" />


## Result
a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.
