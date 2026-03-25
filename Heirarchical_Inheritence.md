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
#Add code here

class Details:

    def __init__(self):
    
        self.name = input("Enter name: ")
        
        self.age = int(input("Enter age: "))


class Employee(Details):
    
    def __init__(self):
    
        super().__init__()
        
        self.emp_id = input("Enter employee ID: ")
        
        self.salary = float(input("Enter salary: "))
    
    def display(self):
        
        print("\nEmployee Details:")
        
        print("Name:", self.name)
        
        print("Age:", self.age)
        
        print("Employee ID:", self.emp_id)
        
        print("Salary:", self.salary)

class Patient(Details):

    def __init__(self):
    
        super().__init__()
        
        self.patient_id = input("Enter patient ID: ")
        
        self.ailment = input("Enter ailment: ")
    
    def display(self):
        
        print("\nPatient Details:")
        
        print("Name:", self.name)
        
        print("Age:", self.age)
        
        print("Patient ID:", self.patient_id)
        
        print("Ailment:", self.ailment)

emp = Employee()

pat = Patient()

emp.display()

pat.display()
## Sample Output
<img width="427" height="616" alt="image" src="https://github.com/user-attachments/assets/467737f2-e6c7-4084-afe1-9af3ab64153b" />


