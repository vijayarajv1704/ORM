# Ex02 Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a student database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![image](https://github.com/SAILESHKUMAR33/ORM/assets/113497410/8e1f95c9-b256-429e-bbad-f4441060a131)


## DESIGN STEPS

### STEP 1:
Clone the repository from github.
### STEP 2:
Create an admin interfacefor Django.
### STEP 3:
Create an app and edit settings.py.
### STEP 4:
Makemigrations and migrate the changes.
### STEP 5:
Create admin user and write pythoncode for admin and models.
### STEP 6:
Make all the migrations to 'myapp'.
### STEP 7:
Create an student database with 10 feilds using runserver command.

## PROGRAM
```
admin.py 

from django.contrib import admin
from .models import student,studentAdmin 
admin.site.register(student,studentAdmin)

models.py

from django.db import models
from django.contrib import admin
class student (models.Model):
    sid=models.CharField(max_length=28)
    name=models.CharField(max_length=30)
    regno=models.IntegerField()
    marks=models.IntegerField()
    email=models.EmailField()

class studentAdmin(admin.ModelAdmin):
    list_display=('sid','name','regno','marks','email')

```


## OUTPUT
![Screenshot 2023-06-11 223610](https://github.com/vijayarajv1704/ORM/assets/121303741/3f1a47d3-40e7-404b-8d7c-eed708e3cd9f)

![Screenshot 2023-06-11 223849](https://github.com/vijayarajv1704/ORM/assets/121303741/fe6e9915-6f9d-46e4-ad8f-7990378d70d0)

## RESULT
The code executed successfully
