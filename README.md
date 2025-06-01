# Ex.08 Design of Interactive Image Gallery
## Date:1-06-2025

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```

<!DOCTYPE html>
<html lang="en">
,
<style>
    * {
        margin: 0%;
        padding: 0%;
        font-family: sans-serif;
    }
    
    h1 {
        color: rgba(223, 255, 199, 0.903);
    }
    
    body {
        background-color: rgb(36, 36, 36);
    }
    
    .gallery {
        width: 80%;
        margin: 100px auto 50px;
        grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    }
    
    .gallery img {
        width: 250px;
        cursor: pointer;
        transition: 1;
    }
    
    .gallery img:hover {
        transform: scale(1.1) rotate(-360deg);
        border-radius: 16px;
        box-shadow: 10px 25px rgba(68, 77, 136, 0.2);
        transition: ease 0.5s;
    }
    
    .ful-img {
        width: 100%;
        height: 100vh;
        background: rgba(0, 0, 0, 0.592);
        top: 0;
        left: 0;
        position: fixed;
        display: none;
        align-items: center;
        justify-content: center;
        z-index: 100;
    }
    
    .ful-img img {
        width: 600px;
        height: 400px;
    }
    
    .ful-img span {
        top: 5%;
        right: 5%;
        position: absolute;
        font-size: 36px;
        color: aliceblue;
        cursor: pointer;
    }
    
    .ful-img span:hover {
        transform: scale(1.8) rotate(-360deg);
        transition: ease 1s;
    }
</style>

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>image gallery</title>
</head>

<body bgcolor="blue">
    <center>
        <h1>IMAGE GALLERY</h1>
    </center>
    <div class="ful-img" id="fulimgbox">
        <center> <img src="/static/8.jpg" id="fulimg"></center>
        <span onclick="closefulimg()">X</span>
    </div>
    <div class="gallery">
        <img src="/static/1.webp" onclick="openfulimg(this.src)">
        <img src="/static/2.jpg" onclick="openfulimg(this.src)">
        <img src="/static/3.jpg" onclick="openfulimg(this.src)">
        <img src="/static/4.jpg" onclick="openfulimg(this.src)">
        <img src="/static/5.jpg" onclick="openfulimg(this.src)">
        <img src="/static/6.jpg" onclick="openfulimg(this.src)">
        <img src="/static/7.jpg" onclick="openfulimg(this.src) ">
        <img src="/static/8.jpg" onclick="openfulimg(this.src) ">

    </div>
</body>
<script>
    var fulimgbox = document.getElementById("fulimgbox");
    var fulimg = document.getElementById("fulimg ");

    function openfulimg(pic) {
        fulimgbox.style.display = "flex "
        fulimg.src = pic
    }

    function closefulimg() {
        fulimgbox.style.display = "none ";

    }
</script>

</html>

```
## OUTPUT:
![image](https://github.com/user-attachments/assets/587aef03-5009-4381-ae08-e3bb686c2793)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
