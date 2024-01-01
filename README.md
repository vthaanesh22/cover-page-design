# cover-page-design
## AIM:
To develop a website to display the cover page design of a book

## Design Steps:

### Step 1:Create a Django Admin project.
### Step 2: Create an app in the Django interface.
### Step 3: Create a folder named 'static' in the app folder.
### Step 4: Create a new HTML file in the static folder.
### Step 5: Write the HTML code with relevant CSS properties.
### Step 6: Choose the appropriate style and color scheme.
### Step 7: Insert the images in their appropriate places.
### Step 8: Publish the website in the LocalHost.

## Code:
``````
<!DOCTYPE html>
<html>
<head>
<title>{% block title %}{% endblock %}</title>
<link href="{% static 'css/bookfrontcover.css' %}" rel="stylesheet">
</head>
<body>
<div id="content">
{% block content %}
{% endblock %}
</div>
</body>
</html>
{% extends "BookFrontCover/base.html" %}
{% block title %}BOOK FRONT COVER App{% endblock %}
{% block content %}
<style>
body {background: #888; height: 100%;}
span {color: #F57D11;}
.book {
display: block;
position: absolute;
height: 850px;
width: 700px;
overflow: hidden;
top: 50%;
left: 50%;
-webkit-transform: translate(-50%,-50%);
-ms-transform: translate(-50%,-50%);
transform: translate(-50%,-50%);
background: #393939;
}
.cover-design {
display: block;
position: absolute;
height: 600px;
width: 600px;
top: 45%;
left: 50%;
-webkit-transform: translate(-50%,-50%);
-ms-transform: translate(-50%,-50%);
transform: translate(-50%,-50%);
font-family: sans-serif;
color: #EEE;
}
.diamond-frame {
position: absolute;
height: 325px;
width: 325px;
top: 64.8%;
left: 14.5%;
-webkit-transform: rotate(45deg) translate(-50%,-50%);
-ms-transform: rotate(45deg) translate(-50%,-50%);
transform: rotate(45deg) translate(-50%,-50%);
border-left: 50px solid #AFA;
border-right: 50px solid #CCC;
border-top: 50px solid #FF7300;
border-bottom: 50px solid #0BF;
}
.box {
position: absolute;
height: 50px;
width: 52px;
z-index: 1000;
}
.a {background: #840; top: -50px; left: -51px;}
.b {background: #b40; top: -50px; right: -51px;}
.c {background: #077; bottom: -50px; right: -51px;}
.d {background: #0A9; bottom: -50px; left: -51px;}
.book-title {
position: absolute;
width: 100%;
font-size: 57px;
top: 45%;
text-align: center;
}
.book-subtitle {
position: absolute;
width: 100%;
font-size: 24px;
top: 55%;
text-align: center;
}
.book-author {
display: block;
position: absolute;
width: 100%;
top: 90%;
text-transform: uppercase;
color: #777;
font-size: 22px;
font-family: sans-serif;
letter-spacing: 2px;
text-align: center;
}
</style>
<div class="book">
<div class="cover-design">
<div class="diamond-frame">
<div class="box a"></div>
<div class="box b"></div>
<div class="box c"></div>
<div class="box d"></div>
</div>
<div class="book-Title"> HTML<span>&</span>CSS </div>
<p class="book-subtitle">design and build websites</p>
</div>
<div class="book-author">Jon Duckett</div>
</div>
{% endblock %}

``````
## Output:
![Screenshot 2024-01-01 151628](https://github.com/vthaanesh22/cover-page-design/assets/139373686/69cca9c8-0903-4535-91ac-f3cb197165ce)


## Result:
The program for designing book front cover page using HTML and CSS is completed successfully.
