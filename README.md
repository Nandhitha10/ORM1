# Ex02 Django ORM Web Application
## Date:22/03/2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

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
'''
models.py
from django.db import models
from django.contrib import admin
class Movie(models.Model):
	Name=models.CharField(max_length=20,primary_key=True)
	Genre=models.CharField(max_length=20)
	Cost=models.IntegerField()
	Run=models.FloatField()
	Rating=models.IntegerField()
class MovieAdmin(admin.ModelAdmin):
	list_display=("Name","Genre","Cost","Run","Rating")

admin.py
from django.contrib import admin
from .models import Movie,MovieAdmin
admin.site.register(Movie,MovieAdmin)
'''
## OUTPUT

![alt text](<Screenshot 2025-03-23 135449.png>)



## RESULT
Thus the program for creating movies database using ORM hass been executed successfully.
