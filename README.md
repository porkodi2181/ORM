# Ex02 Django ORM Web Application
## Date: 22/04/2025
## Name: PORKODI B
## REF.NO 212224240114

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).



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
Models.py

from django.db import models
from django.contrib import admin
class Movie (models.Model):
    mid=models.IntegerField()
    mname=models.CharField(max_length=100)
    collection=models.IntegerField()
    year=models.IntegerField()
    rating=models.FloatField()
    
class MovieAdmin(admin.ModelAdmin):
    list_display=('mid','mname','collection','year','rating')

Adimin.py

from django.contrib import admin
from .models import Movie,MovieAdmin
admin.site.register(Movie,MovieAdmin)

```

## OUTPUT

![Screenshot 2025-04-22 101719](https://github.com/user-attachments/assets/31eb190b-b768-4851-9541-9619d307062a)

![Screenshot 2025-04-12 142639](https://github.com/user-attachments/assets/2557f214-5212-4fc2-b972-34f84c6e0a5d)

## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
