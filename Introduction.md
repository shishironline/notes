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

The result of running this:

>$Enter your password.

>shishir

>$Access denied

>$Enter your password.

>12345

>$Access denied

>$Enter your password.

>Password

>$Access granted

It needs to be modified in order to run properly

The way out is to use `elif` instead of using `if` second time.

Then it works correctly:

$ python Example-2.py

>Enter your password.

>shishir

>Access denied

>Enter your password.

>12345

>That password is one that an idiot puts on their luggage.

>Enter your password.

>Password

>Access granted

