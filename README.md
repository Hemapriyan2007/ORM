# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![435202019-d9ab972b-b80e-402c-8d8d-59a5ffde8b00](https://github.com/user-attachments/assets/ae94eb1d-c32a-4a6e-8338-36f72ebf72e4)



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
