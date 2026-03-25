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

