# Ex.08 Design of Interactive Image Gallery

## AIM
  To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS

## Step 1:

Clone the github repository and create Django admin interface

## Step 2:

Change settings.py file to allow request from all hosts.

## Step 3:

Use CSS for positioning and styling.

## Step 4:

Write JavaScript program for implementing interactivit

## Step 5:

Validate the HTML and CSS code

## Step 6:

Publish the website in the given URL.

## PROGRAM
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gallery</title>
    <style>
        #flexbox
        {
            padding: 170px;
            background-repeat: no-repeat;
            background-size: cover;
        }
        
        #container
        {
            gap: 20px;
            display: flex;
            justify-content: center;
            padding: 10px;
            box-shadow:0 2px 3px;
        }
        .img
        {
            height: 300px;
            width: 300px;
            /* transform: rotate(-10deg); */
            image-rendering:optimizeQuality;    
            border: 2px inset whitesmoke;    
            border-radius: 10px;
            box-shadow:  0 0 10px black ;
            transition: 0.5s;
        }
        .img:hover
        {
            content: 'hello';
            transform: scale(1.3);
        }
        #divs
        {
            display: inline;
        }
        #image
        {
            z-index: 100;
            display: none;
            background: rgba(0,0,0,0.5);
            position: fixed;
            width: 100%;
            /* transform: rotate(20deg); */
            height: 100%;
            top: 0;
            bottom: 0;
            align-items: center;
            justify-content: center;    
        }
        #image img{
            width: 600px;
            height: auto;
        }
        
    </style>
</head>
<body>
    <section id="image">
            <img src="1.jpeg" alt="" id="display" onclick="closes()">
    </section>
<div id="flexbox">

    <h1 align="center" ><span id="title">My Image Gallery </span></h1>

    <div id="container">
        <div class="divs"><img class="img" src="1.jpg" onclick="opens(this.src)" alt=""></div>
        <div class="divs"><img class="img" src="2.jpg" onclick="opens(this.src)"   alt=""></div>
        <div class="divs"><img class="img" src="3.jpg"  onclick="opens(this.src)"  alt=""></div>
        <div class="divs" ><img class="img" src="4.jpg" onclick="opens(this.src)"   alt=""></div>
    </div>
    
    
</div>
<footer align="center" style="background-color:grey">
    <p>Designed & Developed by GOWTHAM &copy; </p>
</footer>
    <script>
            var a =document.getElementById("image");
            var b=document.getElementById("display");
            function opens(c)
            {
                a.style.display='flex';
                b.src=c;
            }
            function closes()
            {
                a.style.display='none';
            }
    </script>
</body>
</html>
```


## OUTPUT
![alt text](<Screenshot 2025-05-21 210334.png>) 
![alt text](<Screenshot 2025-05-21 210030.png>) 
![alt text](<Screenshot 2025-05-21 210128.png>) 
![alt text](<Screenshot 2025-05-21 210217.png>) 
![alt text](<Screenshot 2025-05-21 210240.png>)


## RESULT
  The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
