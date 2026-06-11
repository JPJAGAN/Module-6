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
