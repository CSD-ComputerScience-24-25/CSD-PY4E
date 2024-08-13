# Exercise 13-3:
Modify person.json and add another field or attribute to the file. When you are done you should print Name, Phone, Email Hide, and the data entered into your new field

```python
import json

# Opening JSON file
f = open('person.json')
data = json.load(f)

# Print items
print('Name:', data["name"])
print('Hide:', data["email"]["hide"])

# Closing file
f.close()
```
