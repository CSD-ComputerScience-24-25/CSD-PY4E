# Exercise 13-4: JSON2
Modify the users.json file to add yourself as a user.  When completed, your program should print out each user, and the total number of users

```python
import json
# Opening JSON file
f = open('users.json')
data = json.load(f)
# Print items
for item in data:
  print('Name', item['name'])
  print('Id', item['id'])
  print('Attribute', item['x'])
# Closing file
f.close()
```