# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
 ![Screenshot_20221218_034006](https://user-images.githubusercontent.com/118344695/208292483-98ae1e04-e346-4300-aedd-c36181460564.png)
## DESIGN STEPS
### STEP 1: 
fork the repository and then clone it into the theia ide

### STEP 2:
create django project then create app and superuser account

### STEP 3:
make changes in settings and type your design code in models and the code in admin and then run the server.
## STEP 4:
login on admin with superuser account and populate the record.

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
###admin side outout
![adminoutput](https://user-images.githubusercontent.com/118344695/208288553-e1ab5add-7fc3-43b5-9749-e3226c7af620.png)



## RESULT
the program executed successfully
