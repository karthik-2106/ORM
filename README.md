# Ex02 Django ORM Web Application
## Date: 18-03-2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
```
admin.py

from django.contrib import admin
from .models import books,booksAdmin
admin.site.register(books,booksAdmin)

models.py

from django.db import models
from django.contrib import admin
class books(models.Model):
	name=models.CharField(max_length=20);
	author=models.CharField(max_length=20);
	id=models.IntegerField(primary_key=True);
	copies=models.IntegerField();
	price=models.IntegerField();
class booksAdmin(admin.ModelAdmin):
	list_display=("name","author","id","copies","price");
```

## OUTPUT





![image](https://github.com/karthik-2106/ORM/assets/150319557/5ebc3fef-00b6-4793-8539-65076eaf86b5)

![Screenshot 2024-03-18 193322](https://github.com/karthik-2106/ORM/assets/150319557/53e8dcaa-cfa2-414b-a462-a911552338a6)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
