# Ex02 Django ORM Web Application
## Date: 15.03.2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).
## ER DIAGRAM
<img width="429" alt="Screenshot 2024-03-21 132847" src="https://github.com/KSIHORE/ORM/assets/151484879/931c1d84-d981-4631-9b30-24f105db672f">
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
NAME:KISHORE.B
REF:212222110020
```
```
admin.py

from django.contrib import admin
from django.contrib import admin
# Register your models here.
from.models import Book,BookAdmin
admin.site.register(Book,BookAdmin) 

models.py 

from django.db import models
from django.db import models
from django.contrib import admin
# Create your models here.
class Book(models.Model):
    book_id= models.IntegerField(primary_key=True)
    book_name= models.CharField(max_length=50)
    publisher_name= models.CharField(max_length=50)
    author_name= models.CharField(max_length=50)
    publish_year= models.DateField()

class BookAdmin(admin.ModelAdmin):
    list_display= ('book_id','book_name','publisher_name','author_name','publish_year')
```
## OUTPUT:
<img width="483" alt="image" src="https://github.com/KSIHORE/ORM/assets/151484879/48d7d7da-8a11-4468-8f1f-3425f979bfed">

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
