# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from github.

### STEP 2:
Create a new app.

### STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Create django app and add student details.

## PROGRAM
## models.py 

from django.db import models

from django.contrib import admin


class Student(models.Model):
    
    referencenumber=models.CharField(primary_key=true,max_length=20,help_text="reference number")
    
    name=models.CharField(max_length=100)
    
    age=models.IntegerField()
    
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
   
   list_display=('referencenumber','name','age','email')


## Admin.py

from django.contrib import admin

from myapp.models import Student,StudentAdmin

admin.site.register(Student,StudentAdmin

## OUTPUT
![Screenshot 2023-05-11 144515](https://github.com/SudharsanamRK/django-orm-app/assets/115523484/e8dd044d-e518-48cf-aa1d-76cc5a1af514)

![Screenshot 2023-05-11 144440](https://github.com/SudharsanamRK/django-orm-app/assets/115523484/8e9d323e-c3ed-4ce0-bbdf-53e26df406a5)

## RESULT
Program successfully executed
