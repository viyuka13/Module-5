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
      class employee:
          def __init__(self):
              print("Employee created.")
          def __del__(self):
              print("Destructor called, Employee deleted.")
      e=employee()
      del e

## 🧪 Output

![image](https://github.com/user-attachments/assets/7a123acf-defd-4ea7-b2b0-1addac8247cc)

## Result
The program successfully demonstrates the working of a constructor and a destructor in a Python class by creating and then deleting an object.
