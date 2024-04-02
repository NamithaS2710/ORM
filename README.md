# Ex02 Django ORM Web Application
## Date: 02.04.2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
#### admin.py
```
from django.contrib import admin

from app1.models import Library
admin.site.register(Library)

```

#### models.py
```
from django.db import models

class Library(models.Model):
    bookid=models.IntegerField()
    isbn=models.IntegerField(primary_key=True)
    bookname=models.CharField(max_length=50)
    authname=models.CharField(max_length=30)
    price=models.FloatField()
```
## OUTPUT
![image](https://github.com/Jai-Pradhiksha/ORM/assets/100289733/3ec12aba-de0b-4859-9c71-53b4fc7ad594)

![image](https://github.com/Jai-Pradhiksha/ORM/assets/100289733/452d060a-ff54-4e7c-b384-90e6412f352c)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
