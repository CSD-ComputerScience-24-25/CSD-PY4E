# Exercise 13-2: XML2
Modify the users.xml file and add yourself as a user.  Make sure your program prints out the added information

```python
import xml.etree.ElementTree as ET

tree = ET.parse('users.xml')
lst = tree.findall('users/user')
print('User count:', len(lst))

for item in lst:
  print('Name', item.find('name').text)
  print('Id', item.find('id').text)
  print('Attribute', item.get('x'))

```