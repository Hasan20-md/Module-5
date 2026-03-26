# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
```
# Base Class
class Details:
    def __init__(self):
        self.name = ""
        self.age = 0

    def getName(self):
        self.name = input("Enter Name: ")

    def getAge(self):
        self.age = int(input("Enter Age: "))


# Derived Class 1
class Employee(Details):
    def __init__(self):
        super().__init__()
        self.employee_id = ""
        self.department = ""

    def getEmployeeDetails(self):
        self.getName()
        self.getAge()
        self.employee_id = input("Enter Employee ID: ")
        self.department = input("Enter Department: ")

    def displayEmployee(self):
        print("\n--- Employee Details ---")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Employee ID:", self.employee_id)
        print("Department:", self.department)


# Derived Class 2
class Patient(Details):
    def __init__(self):
        super().__init__()
        self.patient_id = ""
        self.disease = ""

    def getPatientDetails(self):
        self.getName()
        self.getAge()
        self.patient_id = input("Enter Patient ID: ")
        self.disease = input("Enter Disease: ")

    def displayPatient(self):
        print("\n--- Patient Details ---")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)


# Main Program
# Employee Object
emp = Employee()
emp.getEmployeeDetails()
emp.displayEmployee()

# Patient Object
pat = Patient()
pat.getPatientDetails()
pat.displayPatient()
```
## Sample Output
<img width="494" height="713" alt="image" src="https://github.com/user-attachments/assets/ce4b3e23-017d-43aa-a13f-26379c25d69e" />

## Result
Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.
