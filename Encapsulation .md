# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
class Rectangle:

    def __init__(self, length=5, breadth=3):
    
        self.__length = length
        
        self.__breadth = breadth
        
        print("Rectangle Created with Length =", self.__length, "and Breadth =", self.__breadth)
        
    # Method to get area (accessing private members)
    def area(self):
    
        return self.__length * self.__breadth


rect = Rectangle()


print("Area of Rectangle:", rect.area())

## Output
Rectangle Created with Length = 5 and Breadth = 3

Area of Rectangle: 15

## Result
The Python program successfully demonstrated Encapsulation, where the private members __length and __breadth are accessed only through methods within the class, preventing direct external access.
