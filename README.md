# Ex02 Django ORM Web Application
# Date:20/09/2024
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
```
admin.py
from django.contrib import admin
from .models import Bankloan,BankloanAdmin
admin.site.register(Bankloan,BankloanAdmin)

models.py
from django.db import models
from django.contrib import admin
class Bankloan(models.Model):
  name=models.CharField(max_length=100)
  accno=models.IntegerField(primary_key="accno")
  ifscno=models.IntegerField()
  mobno=models.IntegerField()
  email=models.EmailField()
   
class BankloanAdmin(admin.ModelAdmin):
  list_display=('name','customer id','dob','mobno','email','loan amount')
 
```
# OUTPUT
![Screenshot 2024-12-07 194812](https://github.com/user-attachments/assets/d5226fe1-e1ce-485f-9c7d-1e504321a66d)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
