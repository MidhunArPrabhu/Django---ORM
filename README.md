# Django ORM Web Application : 

## AIM :

To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM :

![mc](https://user-images.githubusercontent.com/118054670/212125614-6b5902b1-2683-4f1d-bfda-79301411e531.png)

## DESIGN STEPS

### STEP 1:

Creating a table using required details in Django--ORM

### STEP 2:

Upload the python code.


### STEP 3:

push the code to github.

## PROGRAM :


admin.py:  

from django.contrib import admin  
from .models import Student,StudentAdmin  


admin.site.register(Student,StudentAdmin)  

manage.py:  

from django.db import models  
from django.contrib import admin  
#Create your models here.  

class Student(models.Model):  
    referencenumber=models.CharField(max_length=10,help_text="Your Reference Number")  
    name=models.CharField(max_length=100)  
    department=models.CharField(max_length=200)  
    age=models.IntegerField()  
    email=models.EmailField()  

class StudentAdmin(admin.ModelAdmin):  
    list_display = ('referencenumber','name','age','department','email')  
#Register your models here.  


## OUTPUT :

![MIDHUN AZHAHU RAJA P Screenshot_Django_Admin](https://user-images.githubusercontent.com/118054670/212101737-685ab9b6-049d-4227-9735-2123494d4bae.png)



## RESULT
