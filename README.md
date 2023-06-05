# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![djangoer](https://github.com/SivaMohan-cloud/django-orm-app/assets/121418870/7ffc074a-5737-4551-9eb7-63da6c6de21b)


## DESIGN STEPS

### STEP 1:

### STEP 2:

### STEP 3:

Write your own steps

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
