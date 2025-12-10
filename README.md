# Ex.05 Book Front Cover Page Design
# Date:05.12.2025
# AIM:
To design a book front cover page using HTML and CSS.

# DESIGN STEPS:
## Step 1:
Create a Django Admin project.

## Step 2:
Create an app in the Django interface.

## Step 3:
Create a folder named 'static' in the app folder.

## Step 4:
Create a new HTML file in the static folder.

## Step 5:
Write the HTML code with relevant CSS properties.

## Step 6:
Choose the appropriate style and color scheme.

## Step 7:
Insert the images in their appropriate places.

## Step 8:
Publish the website in the LocalHost.

# PROGRAM:
```
views.py:

from django.shortcuts import render
def book_cover(request):
    return render(request,'cover.html')

```

```
urls.py:

from django.contrib import admin
from django.urls import path
from bookapp import views
urlpatterns = [
    path('admin/', admin.site.urls),
    path('',views.book_cover),
]

```

```
cover.html:

{% load static %}
<html>

<head>
    <title>Book Cover</title>
    <style>
        .border{
            position: absolute;
            border:2px solid black;
            height:95%;
            width:95%;
            left: 2.1%;
            bottom: 2.5%;
        }
        .bg {
            position: relative;
            background-image: url("{% static 'green.jpeg' %}");
            height: 100%;
            width: 35%;
            margin-left: 33%;
        }

        .sticker {
            position: absolute;
            left: 5%;
            top: 4%;
            border-radius: 100%;
            background-color: #6b9071;
            border: 3px solid #6b9071;
            height: 16%;
            width: 22%;
            text-align: center;

        }

       .bg h6 {
            position: absolute;
            margin-top: 7%;
            color: white;
            font-size: 12px;
            line-height: 20px;
            letter-spacing: 13x;
            right: 5%;
        }

        .bg img {
            position: absolute;
            height: 50%;
            width: auto;
            right: -5%;
            top: 23%;

        }

        .bg pre {
            position: absolute;
            font-size: 40px;
            font-family: Georgia, 'Times New Roman', Times, serif;
            line-height: 70px;
            letter-spacing: 10px;
            top: 20%;
            left: -110px;
        }

        .bg h5 {
            position: absolute;
            bottom: 3%;
            left: 30%;
            font-size: 20px;
            letter-spacing: 5px;
            font-family: serif;
            font-weight: 100;
        }

        .bg h4 {
            position: absolute;
            bottom: 13%;
            left: 8%;
            font-size: 22px;
            line-height: 30px;
            letter-spacing: 3px;
            word-spacing: 3px;
            font-style: italic;
            font-family: 'Times New Roman', Times, serif;
            font-weight: lighter;
        }
        .one{
            position: absolute;
            bottom:11%;
            border:1px solid black;
            width:50%;
            left:25.8%;
        }
        .two{
            position: absolute;
            bottom:5%;
            border:1px solid black;
            width:50%;
            left:25.8%;
        }
    </style>
</head>

<body>
    <div class="bg">
        <div class="border"></div>
        <PRE>
        THE 
        COURAGE 
        TO BE 
        DISLIKED
        </PRE>
        <img src="{% static 'waves.png' %}">
        <div class="sticker">
            <h6>
                THE<br>
                INTERNATIONAL<br>
                BEST
                SELLER<br>
                3M
                COPIES <br>
                SOLD
            </h6>
        </div>
        <h4>"The Japanese Phenomenon That<br>
            Shows You How to Change Your Life <br>
            and Achieve Real Happiness"</h4>
            <hr class="one">
            <h5>ICHIRO KISHIMI</h5>
            <hr class="two">
    </div>
</body>

</html>
```
# OUTPUT:
<img width="1913" height="1017" alt="Screenshot 2025-12-10 125104" src="https://github.com/user-attachments/assets/444a8651-2d6d-41a0-b3a4-57823dd7a5ae" />

# RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.

