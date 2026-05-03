# Ex02 Django ORM Web Application
## Date: 3.05.2026

## AIM
To develop a Django application to store and retrieve data from Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
<img width="1039" height="575" alt="image" src="https://github.com/user-attachments/assets/0d3f6e5b-df53-47ac-9cd5-8b86c2f3a259" />


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
models.py
from django.db import models
from django.contrib import admin
class Movie(models.Model):
    title = models.CharField(max_length=255, help_text="Movie Title")
    director = models.CharField(max_length=100, help_text="Director Name")
    release_date = models.DateField(help_text="Release Date")
    genre = models.CharField(max_length=50, help_text="Movie Genre")
    rating = models.DecimalField(max_digits=3, decimal_places=1, help_text="Movie Rating (e.g., 8.5)")
    duration = models.IntegerField(help_text="Duration in Minutes")

class MovieAdmin(admin.ModelAdmin):
    list_display = ('title', 'director', 'release_date', 'genre', 'rating', 'duration')
# Create your models here.

```


## OUTPUT

<img width="1914" height="1107" alt="image" src="https://github.com/user-attachments/assets/7ed90cbf-6ac5-41ed-8e16-420d28238ec8" />



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
