# Ex02 Django ORM Web Application
## Date: 15.09.2025

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
models.py
from django.db import models
from django.contrib import admin
class car(models.Model):
    Model=models.CharField(max_length=10)
    car_no=models.IntegerField(primary_key=True)
    quality=models.CharField(max_length=10)
    year_prod=models.IntegerField()
    color=models.CharField()
class carAdmin(admin.ModelAdmin):
    list_display=["model","car_no","quality","year_prod","color"]
admin.py
from django.contrib import admin
from.models import car,carAdmin
admin.site.register(car,carAdmin)
```

## OUTPUT
![alt text](screenshot(1).jpg)



## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
