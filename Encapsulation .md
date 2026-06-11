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
