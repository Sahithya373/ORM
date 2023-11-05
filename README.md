# Ex02 Django ORM Web Application
## Date: 07/10/2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

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
# Admin.py
```
from django.contrib import admin
from .models import Player,PlayerAdmin
admin.site.register(Player,PlayerAdmin)

```
# Models.py
```
from django.db import models
from django.contrib import admin
class Player(models.Model):
    Player_Name=models.CharField(max_length=50)
    Jersy_No=models.IntegerField()
    Team=models.CharField(max_length=20)
    Height=models.IntegerField()
    Position=models.CharField(max_length=100)

class PlayerAdmin(admin.ModelAdmin):
    list_display=('Player_Name','Jersy_No','Team','Height','Position')

```


## OUTPUT

![Screenshot (21)](https://github.com/Sahithya373/ORM/assets/147017926/f5ce90ea-018c-4fea-a138-6f6b197305ab)

![Screenshot (22)](https://github.com/Sahithya373/ORM/assets/147017926/c13a2098-5397-430d-bf36-013a14fa6a85)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
