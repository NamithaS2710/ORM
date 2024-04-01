# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

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
```
ADMIN.PY
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

MODELS.PY
from django.db import models
from django.contrib import admin
class Employee(models.Model):
    empid=models.IntegerField()
    empname=models.CharField(max_length=20)
    dept=models.CharField(max_length=10)
    salary=models.FloatField()
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('empid','empname','dept','salary')    
```

## OUTPUT
![Screenshot 2024-04-01 203223](https://github.com/NamithaS2710/ORM/assets/133190822/b624a8da-ee0d-414f-82b0-94a8db4fae39)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
