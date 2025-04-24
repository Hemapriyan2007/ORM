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
models.py
from django.db import models
from django.contrib import admin
class Movie(models.Model):
    mid=models.IntegerField()
    mname=models.CharField(max_length=100)
    collection=models.IntegerField()
    year=models.IntegerField()
    rating=models.FloatField()

class MovieAdmin(admin.ModelAdmin):
    list_display=('mid','mname','collection','year','rating')

admin.py
from django.contrib import admin
from .models import Movie,MovieAdmin
admin.site.register(Movie,MovieAdmin)

```
# OUTPUT
![alt text](hema-1.png)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
