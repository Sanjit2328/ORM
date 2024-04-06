# Ex02 Django ORM Web Application
## Date: 06.04.24

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
### models.py:
from django.db import models
from django.contrib import admin
# Create your models here.
class Employee(models.Model):
    empid=models.IntegerField()
    empname=models.CharField(max_length=20)
    dept=models.CharField(max_length=10)
    salary=models.FloatField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('empid','empname','dept','salary')

### admins.py:
from django.contrib import admin

from .models import Employee,EmployeeAdmin
# Register your models here.
admin.site.register(Employee,EmployeeAdmin)

## OUTPUT

Include the screenshot of your admin page.


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
