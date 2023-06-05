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
![image](https://github.com/SAILESHKUMAR33/ORM/assets/113497410/f6d9493f-1375-46cf-8a88-53c3f7ce3d8e)



## RESULT
The code executed successfully
