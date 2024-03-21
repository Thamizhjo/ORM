# Ex02 Django ORM Web Application
## Date: 15/03/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram


![entity relationship-1](https://github.com/Henriprasath/ORM/assets/144979077/38582397-61f3-44d7-ba5f-652d496fdfce)


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
```
from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
      sno=models.IntegerField(primary_key="sno");
      name=models.CharField(max_length=50);
      author=models.CharField(max_length=70);
      price=models.IntegerField();
      publisher=models.CharField(max_length=60);

class Book_DBAdmin(admin.ModelAdmin):
    list_display=("sno","name","author","price","publisher");
```
### admin.py:
```
from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)
```
## OUTPUT

![web 2](https://github.com/Thamizhjo/ORM/assets/123891476/696c7cc6-954d-4883-91a4-49f8ecb6418c)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
