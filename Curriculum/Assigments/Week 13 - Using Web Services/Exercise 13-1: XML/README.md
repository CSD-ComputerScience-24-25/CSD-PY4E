# Exercise 13-1: XML
Your job is to modify person.xml and add a field or property, then find and print the phone number as well as the added data
```python
import xml.etree.ElementTree as ET

tree = ET.parse('person.xml')
print('Name:', tree.find('name').text)
print('Attr:', tree.find('email').get('hide'))
```