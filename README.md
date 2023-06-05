# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![djangoer](https://github.com/SivaMohan-cloud/django-orm-app/assets/121418870/7ffc074a-5737-4551-9eb7-63da6c6de21b)


## DESIGN STEPS
##STEP 1:
clone the repository from github.

##STEP 2:
create an admin interface for django

##STEP 3:
create an app and edit settings.py

##STEP 4:
make migrations and migrate the changes.

##STEP 5:
create admin user and write python code for admin and models.

##STEP 6:
make all the migrations to 'myapp'.

##STEP 7:
create an student database with 10 fields using runserver command.

## PROGRAM

Include your code here
## Models.py
```py
from django.db import models
from django.contrib import admin

# Create your models here.
class Student (models.Model):
    referencenumber=models.CharField(primary_key=True,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    phoneno=models.IntegerField()

class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email','phoneno')
```
## Admin.py
```py
from django.contrib import admin
from .models import Student,StudentAdmin


# Register your models here.
admin.site.register(Student,StudentAdmin)
```


## OUTPUT
##Server Output:
![djangooutput1](https://github.com/SivaMohan-cloud/django-orm-app/assets/121418870/f927cc24-d52c-43cc-a8d8-64fbbf47c09e)

##Client Output:
![djangooutput2](https://github.com/SivaMohan-cloud/django-orm-app/assets/121418870/d6bd549e-97a2-4387-a6e5-4314ac656e1a)

## RESULT
The program for creating an student database using ORM is executed sucessfully.
