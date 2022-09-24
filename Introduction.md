---
id: n25s2mqlsvrtggdemn3pyrd
title: Introduction
desc: ''
updated: 1664014332630
created: 1664014169747
---
A program is given on this page, as an example.

```
passwordFile = open('SecretPasswordFile.txt')

secretPassword = passwordFile.read()

print('Enter your password.')

typedPassword = input()

if typedPassword == secretPassword:

  print('Access granted')
  
  if typedPassword == '12345':
  
    print('That password is one that an idiot puts on their luggage.')

else:

  print('Access denied')
```
Add one text file SecretPasswordFile.txt in the current folder with password as its only content.

It needs to be modified in order to run properly
