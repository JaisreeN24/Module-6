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
      from abc import ABC, abstractmethod
      import math
      class Shape(ABC):
          @abstractmethod
          def calculate_area(self):
              pass
      class Rectangle(Shape):
          def __init__(self, length=1, breadth=1):
              self.length = length
              self.breadth = breadth
          def calculate_area(self):
              return self.length * self.breadth
      class Circle(Shape):
          def __init__(self, radius=1):
              self.radius = radius
          def calculate_area(self):
              return math.pi * self.radius ** 2
      rect = Rectangle(4, 5)
      circle = Circle(3)
      print("Rectangle Area:", rect.calculate_area())
      print("Circle Area:", circle.calculate_area())

## Output
![image](https://github.com/user-attachments/assets/900b5616-e4ec-4b89-9768-8be0d6af84a6)

## Result
Thus, To create an abstract class named Shape with an abstract method calculate_area, and implement this method in two subclasses: Rectangle and Circle is verified and executed successfully.

