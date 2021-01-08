# Web Design for a Manufacturing Company
## AIM: 
To design a static website for a chip manufacturing company.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.

## PROGRAM:

### base.html
```
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <title> Prasanna Corp Limited </title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel="icon" href="{% static 'img/icon.png' %}" type="image/x-icon">

</head>

<body>
    <div class="container">
        <div class="chip1">
            Prasanna Corp Limited
        </div>
        <div class="menu">
            <div class="menuitem"><a href="/home">Home</a></div>
            <div class="menuitem"><a href="/products">Products</a></div>
            <div class="menuitem"><a href="/people">People</a></div>
            <div class="menuitem"><a href="/contactus">Contact Us</a></div>
        </div>
        <div class="content">
            {% block content %}
            {% endblock  %}
        </div>
        <div class="footer">
            Copyright © 2021 PRAS Private Limited, Developed by Prasanna
        </div>
    </div>
</body>

</html>

```

### home.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="homecontent">    
    <h1>About Us</h1>
    <img src="/static/img/CHIP4.jpg" alt="Building">
    <div class="contenttext">
    Prasanna Corp Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications that serve the data center, networking, software, broadband, wireless, and storage and industrial markets. Common applications for its products include: data center networking, home connectivity, broadband access, telecommunications equipment, smartphones, base stations, data center servers and storage, factory automation, power generation and alternative energy systems, displays, and mainframe operations and management, and application software development. Some of Silicon's core technologies and products include:
    <ul>
        <li>Memory Chips</li>
        <li>SATA HDD</li>
        <li>SATA SSD </li>
        <li>Broadband Modems</li>
        <li>Wifi Devices</li>
        <li>Switching Devices</li>
        <li>Optical Sensors</li>
    </ul> 
    </div>
    </div>
{% endblock  %}
```
### products.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="productcontent">    
    <h1>Our Premium Products</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/4gb laptop memory.jpg" alt="product image">
            </div>
            <div class="itemname">4GB DDRA4 laptop memory</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/1tb laptop hdd.jpg"  alt="product image">
            </div>
            <div class="itemname">1TB Laptop HDD</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/graphic.jpg"  alt="product image">
            </div>
            <div class="itemname">Graphic card</div>
            <div class="itemprice">Price: Rs.30000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/mouse.jpg"  alt="product image">
            </div>
            <div class="itemname">mouse</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/speaker.jpg"  alt="product image">
            </div>
            <div class="itemname">speaker</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/ram rgb.jpg"  alt="product image">
            </div>
            <div class="itemname">ram rgb</div>
            <div class="itemprice">Price: Rs.4000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/rgb keybord.jpg"  alt="product image">
            </div>
            <div class="itemname">RGB Keyboard</div>
            <div class="itemprice">Price: Rs.2500.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/sata ssd.jpg"  alt="product image">
            </div>
            <div class="itemname">SATA SSD (samsung)</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/boom headset.jpeg"  alt="product image">
            </div>
            <div class="itemname">Boom Headset</div>
            <div class="itemprice">Price: Rs.3000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/pendrive.jpg"  alt="product image">
            </div>
            <div class="itemname">pendrive 64gb</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/iot board.jpg"  alt="product image">
            </div>
            <div class="itemname">iot-board</div>
            <div class="itemprice">Price: Rs.5500.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/intel i9 9900k.jpg"  alt="product image">
            </div>
            <div class="itemname">intel i9 9900k processor</div>
            <div class="itemprice">Price: Rs.36000.00 </div>
        </div>
    </div>
    </div>
{% endblock  %}
```
### people.html
```
{% extends "website/base.html" %}

{% block content %}
<div class="peoplecontent">
    <h1>Our Crew</h1>
    <div class="crewmembers">
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/prasanna1.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">PRASANNAKUMAR</div>
            <div class="designation">C.E.O PRAS CORP</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/shoheel.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">SHOHEEL</div>
            <div class="designation">FRONTEND DEV</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/varma.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">VARMA</div>
            <div class="designation">TECHNICAL TEAM</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/aadhi1.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">AADHI</div>
            <div class="designation"> R & D HEAD </div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/prashethaa.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">PRASHEETHA</div>
            <div class="designation"> DESIGN TEAM </div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/vincent.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">VINCENT</div>
            <div class="designation"> MARKETING HEAD </div>
        </div></div>
    </div>
    {% endblock  %}
```
### contactus.html
```
{% extends "website/base.html" %}

{% block content %}
<h1>contactus:</h1>
<h2>emailid:prasannakumar10418@gmail.com</h2>
<h3>phone no:8667387776</h3>
{% endblock  %}
```
## OUTPUT:
![output](./static/img/o1.png)

![output](./static/img/o2.png)
![output](./static/img/o3.jpg)
![output](./static/img/o5.png)

## CODE VALIDATION REPORT:
![output](./static/img/r1.png)

![output](./static/img/r2.png)
![output](./static/img/r3.png)
![output](./static/img/r4.png)
![output](./static/img/r5.jpg)
## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://prasanna.student.saveetha.in:8000/. HTML code is validated.