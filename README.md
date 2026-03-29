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

#Add code here

name = input("Enter student name: ")

class Student:

    def __init__(self):
    
        self.a = name

    def show(self):
        
        print("This is non-parameterized constructor")
        
        print("Welcome", self.a)

s = Student()
s.show()

## Output
<img width="546" height="167" alt="image" src="https://github.com/user-attachments/assets/1312a7c4-78b0-425a-b841-2432d85f56a8" />


## Result
Thus the program was successfully executed and obtained the result.


# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method:
   - Initialize an instance variable `status` with the value `"Alive"`.
   - Print the value of `status`.
3. Define the `__del__` method:
   - Print a message indicating the object is being destroyed.
4. Outside the class:
   - Create an instance of the `Demo` class.
   - Delete the object using the `del` keyword.
## Program
#Add code Here

class Demo:

    def __init__(self):
    
        self.status = "Alive"
        
        print(self.status)
    
    def __del__(self):
        
        print("Object is destroyed")

obj = Demo()

del obj

## 🧪 Output
<img width="349" height="127" alt="image" src="https://github.com/user-attachments/assets/d63c2270-bffb-4c12-b3a6-587921e88415" />


## Result
Thus the program was successfully executed and obtained the result.




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


# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
Add code here

class Person:
    
    def __init__(self, name):
    
        self.name = name
    
    def getName(self):
        
        return self.name

class Child(Person):
    
    def __init__(self, name, age):
    
        super().__init__(name)
        
        self.age = age
    
    def getAge(self):
        
        return self.age

class Grandchild(Child):
    
    def __init__(self, name, age, location):
    
        super().__init__(name, age)
        
        self.location = location
    
    def getLocation(self):
        
        return self.location

name = input()

age = int(input())

location = input()

person = Grandchild(name, age, location)

print("Name:", person.getName())

print("Age:", person.getAge())

print("Location:", person.getLocation())

## Sample Output

<img width="419" height="622" alt="image" src="https://github.com/user-attachments/assets/388d13dd-f92e-42b8-babf-207d4991062f" />



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
##Add code here

class Calculation1:

    def Summation(self, a, b):
    
        return a + b

class Calculation2:

    def Subtraction(self, a, b):
    
        return a - b

class Derived(Calculation1, Calculation2):

    def Division(self, a, b):
    
        return a / b

a = float(input())

b = float(input())

obj = Derived()

print("Addition:", obj.Summation(a, b))

print("Subtraction:", obj.Subtraction(a, b))

print("Division:", obj.Division(a, b))
## Output Example
<img width="329" height="273" alt="image" src="https://github.com/user-attachments/assets/c37804ce-a352-4de0-b946-392a42980ba5" />



