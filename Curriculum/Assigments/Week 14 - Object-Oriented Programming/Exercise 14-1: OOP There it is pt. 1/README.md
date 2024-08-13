# Exercise 14-1: OOP There it is pt. 1
For this exercise we are going to make our own class.  This class is going to be a square class that stores information common to squares such as width, height.  You should add the code below to your main file, and instantiate a ```Square()``` object.  Your code should print out the object type, the height, the width and the color.

```python
class Square():
  def __init__(self, height: int, width: int, color: str) -> None:
    self.height = height
    self.width = width
    self.color = color
```