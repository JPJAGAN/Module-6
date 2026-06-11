## Python OOP: Polymorphism with Classes
## AIM
To create two specific classes — Beans and Mango. Then, create a generic function that can accept any object and determine its type (Fruit or Vegetable) and color, using polymorphism.

## ALGORITHM
Create Class Beans:

Define type() method that prints "Vegetable".
Define color() method that prints "Green".
Create Class Mango:

Define type() method that prints "Fruit".
Define color() method that prints "Yellow".
Define Generic Function func(obj):

Call obj.type() and obj.color() — this works with both Beans and Mango objects, showcasing polymorphism.
Create Objects:

Instantiate Beans and Mango.
Pass them to func() and execute the program.
## Program
```
class Beans(): 
     def type(self): 
       print("Vegetable") 
     def color(self):
       print("Green") 
class Mango(): 
     def type(self): 
       print("Fruit") 
     def color(self): 
       print("Yellow")
obj_beans = Beans() 
obj_mango = Mango()
for func in (obj_beans,obj_mango): 
    func.type()
    func.color()
```
## Output
<img width="587" height="290" alt="{1963F0B3-CD5F-4E9A-966E-5CCF2D0A5D7E}" src="https://github.com/user-attachments/assets/9057b952-2412-43c6-8400-9fdf409ffa03" />

## Result
Thus,the program is executed successfully.
