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
    # Base class
    class Details:
        def __init__(self, name, age):
            self.name = name
            self.age = age
    
        def getName(self):
            return self.name
    
        def getAge(self):
            return self.age
    
    
    # Derived class 1
    class Employee(Details):
        def __init__(self, name, age, employee_id, department):
            super().__init__(name, age)
            self.employee_id = employee_id
            self.department = department
    
        def getEmployeeDetails(self):
            print(f"Employee Name: {self.getName()}")
            print(f"Employee Age: {self.getAge()}")
            print(f"Employee ID: {self.employee_id}")
            print(f"Department: {self.department}")
    
    
    # Derived class 2
    class Patient(Details):
        def __init__(self, name, age, patient_id, disease):
            super().__init__(name, age)
            self.patient_id = patient_id
            self.disease = disease
    
        def getPatientDetails(self):
            print(f"Patient Name: {self.getName()}")
            print(f"Patient Age: {self.getAge()}")
            print(f"Patient ID: {self.patient_id}")
            print(f"Disease: {self.disease}")
    
    
    def main():
        print("Enter Employee Details:")
        emp_name = input("Name: ")
        emp_age = input("Age: ")
        emp_id = input("Employee ID: ")
        emp_dept = input("Department: ")
    
        employee = Employee(emp_name, emp_age, emp_id, emp_dept)
    
        print("\nEnter Patient Details:")
        pat_name = input("Name: ")
        pat_age = input("Age: ")
        pat_id = input("Patient ID: ")
        pat_disease = input("Disease: ")
    
        patient = Patient(pat_name, pat_age, pat_id, pat_disease)
    
        print("\n--- Employee Details ---")
        employee.getEmployeeDetails()
    
        print("\n--- Patient Details ---")
        patient.getPatientDetails()
    
    
    if __name__ == "__main__":
        main()

## Sample Output
![image](https://github.com/user-attachments/assets/294bffe7-86de-4d0a-b2bc-894e1aa15894)
#Result
The program defines a Node class for doubly linked list nodes and a DoublyLinkedList class to manage the list. It inserts elements at the end, maintaining previous and next references, and prints the elements in order when traversed. The output correctly displays the inserted elements in sequence.
