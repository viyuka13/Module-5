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
class person:
    def __init__(self,name):
        self.name=name
    
class Age(person):
    def __init__(self,name,age):
        super().__init__(name)
        self.age=age
        
class ID(Age):
    def __init__(self,name,age,id):
        super().__init__(name,age)
        self.id=id
        
    def display(self):
        print(self.name , self.age , self.id)
        
name=input()
age=int(input())
id=int(input())
p=ID(name,age,id)
p.display()


## Sample Output
![image](https://github.com/user-attachments/assets/098c4d79-480c-47c1-9a7f-5b26e707955b)
##Result
The program defines a Node class for doubly linked list nodes and a DoublyLinkedList class to manage the list. It inserts elements at the end, maintaining previous and next references, and prints the elements in order when traversed. The output correctly displays the inserted elements in sequence.
