# Ex02 Django ORM Web Application
# Date:
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
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
### models.py:
```py
from django.db import models
from django.contrib import admin
#creat your modelsr=models.CharField(primary_key=True,max_lenght=20,help_text="referencenumber")
    name=models.CharFiled(max_lenght=100)
    age=models.IntegerFiled()
    email=models.EmailFiled()
    phonenumber=mopdels.IntegerFiled()

    class StudentAdmin(admin.ModelAdmin):
       list_display=('referencenumber','name','age','email','phonenumber')
```
### admin.py:
```py
class student (models.Model):
    referencenumbe
from django.contrib import admin
from .models import student,StudentAdmin

# Register your models here.
admin.site.register(student,StudentAdmin)
```
# OUTPUT
![hdrdg5au](https://github.com/user-attachments/assets/4d912c6f-05df-412f-9793-c084a12dd630)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
