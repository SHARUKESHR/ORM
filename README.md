# Ex02 Django ORM Web Application
## Date:18/10/2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

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
Execute Django admin and create 10 Football players

## PROGRAM
```
MODEL.PY
from django.db import models
from django.contrib import admin
class Football_player (models.Model):
    name=models.CharField(max_length=20)
    age=models.IntegerField()
    email=models.EmailField()
    height=models.IntegerField()
    weight=models.IntegerField()

class Football_playerAdmin(admin.ModelAdmin):
    list_display=['name','age','email','height','weight']

ADMIN.PY
from django.contrib import admin
from .models import Football_player,Football_playerAdmin
admin.site.register(Football_player,Football_playerAdmin)
```



## OUTPUT
![Screenshot 2023-10-13 143236](https://github.com/SHARUKESHR/ORM/assets/144870484/59a2bc2c-bf6f-4b9f-8caf-ba34b52f6d98)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
