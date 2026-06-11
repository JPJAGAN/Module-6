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
