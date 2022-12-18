# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:

### STEP 2:

### STEP 3:

Write your own steps

## PROGRAM
```
from django.db import models
from django.contrib import admin
class patient_details(models.Model):
    patientid = models.CharField(primary_key = True,max_length=8)
    patientname = models.CharField(max_length=100)
    age = models.IntegerField()
    mobileno = models.IntegerField()
    diseases = models.CharField(max_length=200)
    address=models.CharField(max_length=200)


class patient_detailsAdmin(admin.ModelAdmin):
    list_display = ('patientid','patientname','age','mobileno','diseases','address')
```


## OUTPUT

![admin side output](adminoutput.png)


## RESULT
the program executed successfully
