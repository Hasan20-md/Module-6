# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
```
# Step 1: Import ABC module
from abc import ABC, abstractmethod
import math

# Step 2: Abstract Class
class Shape(ABC):
    
    @abstractmethod
    def calculate_area(self):
        pass


# Step 3: Rectangle Class
class Rectangle(Shape):
    def __init__(self):
        self.length = 5
        self.breadth = 3

    def calculate_area(self):
        return self.length * self.breadth


# Step 4: Circle Class
class Circle(Shape):
    def __init__(self):
        self.radius = 4

    def calculate_area(self):
        return math.pi * self.radius ** 2


# Step 5: Create objects and call methods
rect = Rectangle()
circ = Circle()

print("Rectangle Area:", rect.calculate_area())
print("Circle Area:", circ.calculate_area())
```

## Output
<img width="450" height="191" alt="image" src="https://github.com/user-attachments/assets/a316c801-8b29-4d65-b422-09081d346713" />

## Result:
An **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`
is created.
