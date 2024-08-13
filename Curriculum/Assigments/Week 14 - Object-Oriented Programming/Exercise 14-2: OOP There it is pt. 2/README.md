# Exercise 14-2: OOP There it is pt. 2
We are going to continue where we left off on the previous exercise, except we are going to move the ```Square()``` class to its own module named shapes, and import it into main.  After that, we are going to create our first class methods to return the perimeter, and the area of our square.  
__Bonus__:  Modify your class so that it won't create unless the width and height are the same.

# Bonus Hint:
You can do it with object.\_\_new\_\_() however, this is run to create the instance in the first place. Because it is normally supposed to return that new instance, you could also choose to return something else (like None).

You could use it like this:
```python
class MyObj:
def __new__(cls, id):
    # ...SQL request with id as key...
    if not rows:
        # no rows, so no data. Return `None`.
        return None

    # create a new instance and set attributes on it
    instance = super().__new__(cls)  # empty instance
    instance.rows = ...
    return instance
  ```
  Credit: https://stackoverflow.com/questions/44139867/dont-create-object-when-if-condition-is-not-met-in-init
