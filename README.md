# Ex02 Django ORM Web Application
## Name: Hemapriyan P
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![image](https://github.com/user-attachments/assets/e39b80d8-daba-4d44-97a0-9974acad7e38)
![WhatsApp Image 2025-03-25 at 08 47 55_c1657002](https://github.com/user-attachments/assets/0394d65a-d5bf-40c5-8309-35c8343a567b)


## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

models.py

from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee ID")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')
```
# OUTPUT
![Screenshot (226)](https://github.com/user-attachments/assets/f7ef3a9d-d0f7-45b6-9bad-e518fc9dd00a)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
