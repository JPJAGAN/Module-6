## Python OOP: Abstract Class & Method Example
## AIM
To create an abstract class named Shape with an abstract method calculate_area, and implement this method in two subclasses: Rectangle and Circle.

## ALGORITHM
Import ABC module:

Use from abc import ABC, abstractmethod to define abstract classes and methods.
Create Abstract Class Shape:

Define an abstract method calculate_area() with @abstractmethod.
Create Subclass Rectangle:

Set default values for length and breadth.
Override calculate_area() to compute the rectangle area.
Create Subclass Circle:

Set default value for radius.
Override calculate_area() to compute the circle area.
Create Objects & Call Methods:

Instantiate Rectangle and Circle.
Call their calculate_area() methods.
## Program
```
from abc import ABC
class Shape(ABC):
    def calculate_area(self):
        pass
class Rectangle(Shape):
    length = 5
    breadth =3 
    def calculate_area(self):
        return self.length * self.breadth

class Circle(Shape):
  radius = 4
  def calculate_area(self):
        return self.radius * self.radius*3.14

rec=Rectangle()
cir=Circle()#object created for the class 'Rectangle'
#object created for the class 'Circle'
print("Area of a rectangle:", rec.calculate_area()) #call to 'calculate_area' method defined inside the class 'Rectangle'
print("Area of a circle:", cir.calculate_area()) #call to 'calculate_area' method defined inside the class 'Circle'.
```
## Output

<img width="1047" height="228" alt="{76997A66-F007-4D3D-B16F-3B1AEE999D49}" src="https://github.com/user-attachments/assets/c1bbccc9-639b-494b-b349-6d8b4b6b3043" />

##Result
Thus, the python program is executed successfully.

## Python OOP: Encapsulation with Private Members
## AIM
To implement Encapsulation in Python by defining a class Rectangle with private member variables __length and __breadth.

## ALGORITHM
Define the Class:

Create a class Rectangle with two private attributes: __length and __breadth.
Initialize Variables:

Use the __init__() constructor to set initial values for __length and __breadth.
Print Values:

Display the private variables from within the class to demonstrate access.
Instantiate the Object:

Create an object of the Rectangle class to trigger the constructor.
## Program
```
class Rectangle:
    def __init__(self, length, width):
        self.__length = length  # Private variable
        self.__width = width    # Private variable
    
    # Method to print private variables
    def print_values(self):
        print(self.__length)
        print(self.__width)

# Create an object of Rectangle class
rect = Rectangle(5, 3)

# Print private values using the method within the class
rect.print_values()

# Attempt to print private values outside the class (will raise an AttributeError)
```
## Output

<img width="1049" height="243" alt="{887D8BBF-23E2-43E8-A77E-05C7FE86E604}" src="https://github.com/user-attachments/assets/1bd7c39c-321c-4bc8-b76c-e482b7579dfd" />

## Result
Thus, the program is executed successfully

## Method Overriding-Fish and Shark Class Inheritance in Python
## AIM:
To write a Python program that demonstrates class inheritance by creating a parent class Fish with a method type, and a child class Shark that overrides the type method.

## ALGORITHM:
Define the Fish class with a method named type() that prints "fish".
Define the Shark class as a subclass of Fish, and override the type() method to print "shark".
Create an instance of the Fish class named obj_goldfish.
Create an instance of the Shark class named obj_hammerhead.
Use a for loop to iterate over both objects.
Within the loop, call the type() method using the loop variable.
Output will demonstrate method overriding: printing "fish" and "shark" accordingly.
## PROGRAM:
```
class Fish:
    def type(self):
        print("fish")


class Shark(Fish):
    def type(self):
        print("shark")


obj_goldfish = Fish()
obj_hammerhead = Shark()

obj_goldfish.type()
obj_hammerhead.type()
```
## OUTPUT

<img width="987" height="332" alt="{DDB9F6EA-600A-4962-B67C-5CFFF575A501}" src="https://github.com/user-attachments/assets/8d2980ba-1a95-4e5c-bafd-003c5b815e1f" />

## RESULT
Thus,the program is executed successfully.

## Python OOP: Operator Overloading (Less Than <)
## AIM
To write a Python program that demonstrates operator overloading by overloading the less than (<) operator using a custom class.

## ALGORITHM
Create Class A:

Define the __init__() method to initialize the object with a value a.
Overload the < Operator:

Define the __lt__() method with logic:
If self.a < o.a, return "ob1 is less than ob2"
Else, return "ob2 is less than ob1"
Create Objects:

Instantiate two objects ob1 and ob2 with values.
Use < Operator:

Use print(ob1 < ob2) to trigger the overloaded behavior.
## Program
```
class A:
    def __init__(self,a):
        self.a=a
    def __gt__(self,other):
        return self.a<other.a
ob1=A(200)
ob2=A(30)
if(ob1<ob2):
    print("ob2 is less than ob1")
else:
    print("ob1 is less than ob1")
```
## Output

<img width="564" height="241" alt="{302284DC-27C4-4D3A-8EA3-EC40B267F192}" src="https://github.com/user-attachments/assets/891fbb90-51fe-4c66-8db7-f84dd5518bc4" />

## Result
Thus,the program is executed successfully.

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
