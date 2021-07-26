# HTML / CSS Projects
*Developed for educational purposes*
## Overview
These are HTML/CSS and Basic JS Projects. Various components including Meida, Navigation, Flex/Grid Layouts, and More. Explore the code below:
### Key
- [Hello World](#hello-world)
- [Navigation](#navigation)
- [Navigation w/ External Stylesheet](#navigation-w-external-stylesheet)
- [Form](#form)
- [List](#list)
- [Table](#table)
- [1-Page Website](#1-page-static-website)
- [Challenges](#challenges)

## Basics
### Hello World
Hello World static website with an external CSS stylesheet.
```html
<html lang="">
<head>
<meta charset="utf-8">
<title></title>
<link rel="stylesheet" type="text/css" href="Basic_CSS_1.css">
</head>
<body>
<div style = "background-color: blue; color: white; text-align:right">
<!-- OPTIONAL CSS
<stlye>
h1 {color: white; background-color: blue; text-align:right;}
</style>
-->
<h1>HELLO YOU COOL PERSON</h1>
<p>This is a test for external styling</p>
</div>
</body>
</html>
```
### Navigation
Navigation layout with inline css styling.
```html
<!DOCTYPE html>
<html lang="">
<head>
<meta charset="utf-8">
<title></title>
</head>
<body>
<style>
.font_1 {
background-color: black;
color: white;
font-size: large;
}

.font_2 {
background-color: darkblue;
color: white;
font-size: medium;
}

.navigation { /* could aslo use 'nav' {} but wanted user decalation for project*/
background-color: darkgrey;
color: white;
text-decoration: none;
font-weight: bold;
}

a {
text-decoration: none;
color: white;
}

/*moved to external sheet
.My_Style {
color: yellow;
}*/

</style>
<nav class="navigation">
<a href="#">HOME</a>
<a href="#">MORE</a>
<a href="#">ABOUT</a>
</nav>

<h2 class="font_1">This element is styled per class attribute font_1</h2>
<h3 class="font_2">This element is styled per class attribute font_2</h3>
<h4 class="font_1">This element is styled per class attribute font_1 even though its h4</h4>

<p class="My_Style">PHONE NUMBER:</p>

</body>
</html>
```
### Navigation w/ External Stylesheet
```html
<!DOCTYPE html>
<html lang="">
<head>
<meta charset="utf-8">
<title></title>
<link rel="stylesheet" type="text/css" href="Basic_CSS_2.css">
</head>
<body>
<nav class="navigation">
<a href="#">HOME</a>
<a href="#">MORE</a>
<a href="#">ABOUT</a>
</nav>

<p class="My_Style">PHONE NUMBER &gt;</p>
<h1>Welcome to this thing</h1>

</body>
</html>
```
### Form
```html
<!--FORM-->

<form action="" method="get">

First Name: <input type="text" name="First_Name"> <br>
Last Name: <input type="text" name="Last_Name"> <br>
Email <input type="text" name="User_Email"> <br>
<input type="submit" value="Submit">

</form>
```
### List
```html
<header></header>

<main>
<!--LISTS-->
<ul>
<li>Flour</li>
<li>Butter</li>
<li>Eggs</li>
<li>Baking Powder</li>
</ul>
<ol>
<li>Flour</li>
<li>Butter</li>
<li>Eggs</li>
<li>Baking Powder</li>
</ol>
</main>

<footer></footer>
```
### Table
```html
<!--TABLE-->

<table>
<th>Name</th>
<th>T-Shirt Size</th>
<th>Email</th>

<tr>
<td>John Doe</td>
<td>Large</td>
<td>johndoe@email.com</td>
</tr>

<tr>
<td>Jane Doe</td>
<td>Medium</td>
<td>janedoe@email.com</td>
</tr>

<tr>
<td>Jimmy Doe</td>
<td>Small</td>
<td>does not have email</td>
</tr>

</table>
```
### 1-Page Static Website 
*Navigation*
```html
<!--MAIN NAVIGATION-->
<section>
<div id="wrapper_1">
<div id="logo">
<img src="../assets/images/logo.png" alt="logo">
</div>

<nav>
<a href="#home" id="link">HOME</a>
<a href="#explore" id="link">EXPLORE</a>
<a href="#contact" id="link">CONTACT</a>
</nav>
</div>
</section>
<!-- END MAIN NAVIGATION-->
```
*Home*
```html
<!--HOME-->
<section>
<div id="home">
<div id="banner">
<img src="../assets/images/banner.jpg" alt="banner image">
</div>

<div id="banner-text">
<h1>Let's talk about that shirt you're wearing.</h1>
<p>(I mean, <strong><em>it looks great</em></strong>, but have you thought about its global impact?)</p>
</div>
</div>
</section>
<!--END HOME-->
```
*Contact*
```html
<!--CONTACT-->
<section id="contact">
<div class="tab tab_2">
<h1>CONTACT</h1>
</div>

<div class="wrapper wrapper_2">
<div id="form">
<h1>Sign up for our newsletter!</h1>
<form action="" method="get">
<span><strong>&nbsp;&nbsp;NAME</strong></span><br><input type="text" name="First_Name"> <br>
<span><strong>&nbsp;&nbsp;AGE</strong></span><br><input type="text" name="Last_Name"> <br>
<span><strong>&nbsp;&nbsp;EMAIL</strong></span><br><input type="text" name="User_Email"> <br>
<input type="submit" value="Submit">
</form>

<!--EMBEDDED VIDEO & MESSAGE-->
<div id="video-section">
<div id="video">
<iframe width="560" height="315" src="https://www.youtube.com/embed/SzcGTd8qWTg" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
<div id="info">
<p>Above is more information on the global impacts <br>of the fast fashion industry. If you would like more <br> information, or to donate & help, please fill out our form.</p>
<p><strong>Thank You.</strong></p>
</div>
</div>
<!--END VIDEO & MESSAGE-->

</div>
</div>
</section>

<!--END CONTACT-->
```
## Challenges
### Center an Image
```html
<!--EXAMPLE OF STYLED IMAGE CENTERED ON PAGE-->
<!DOCTYPE html>
<html>
<head>
<title>CENTER IMAGE</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
img {
display: block;
margin-left: auto;
margin-right: auto;
width: 25%;
filter: invert(100%); /* inverts image */
border-radius: 25px; /* rounded corners */
}
</style>
</head>

<body>
<img src="../assets/drink.jpg" alt="">
</body>
</html>
```
### Embed a Video Loop
```html
<!--EMBED VIDEO AUTOPLAY // LOOP // MUTED-->
<!DOCTYPE html>
<html>
<head>
<title> </title>
</head>
<body>
<video width="320" height="240" controls autoplay muted loop>
<source src="../assets/city.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>
</body>
</html>
```
### Footer
```html
<!--Footer Example-->
<!DOCTYPE html>
<html>
<head>
<title>CENTER IMAGE</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>

footer {
text-align: center;
padding: 3px;
background-color: teal;
color: white;
}

.column {
float: left;
width: 50%;
font-weight: bold;
}

/* Clear floats after the columns */
.row:after {
content: "";
display: table;
clear: both;
}
</style>
</head>

<body>
<div class="section">
<footer>
<div class="row">
<div class="column">
<a href="#">This is a link</a>
<a href="#">This is a link</a>
<a href="#">This is a link</a>
</div>
<div class="column">
<p>This is more information</p>
<p>This is more information</p>
<p>This is more information</p>
<p>This is more information &copy;</p>
</div>
</div>
</footer>
</div>
</body>
</html>
```
### Paragraph Hover Effect
```html
<!--IMG OVERLAY FADE-->
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
.container {
position: relative;
width: 50%;
}

.image {
display: block;
width: 100%;
height: auto;
}

.overlay {
position: absolute;
top: 0;
bottom: 0;
left: 0;
right: 0;
height: 100%;
width: 100%;
opacity: 0;
transition: .5s ease;
background-color: #008CBA;
}

.container:hover .overlay {
opacity: 1;
}

.text {
color: white;
font-size: 20px;
position: absolute;
top: 50%;
left: 50%;
-webkit-transform: translate(-50%, -50%);
-ms-transform: translate(-50%, -50%);
transform: translate(-50%, -50%);
text-align: center;
}
</style>
</head>

<body>
<h2>Fade in Overlay</h2>
<p>Hover over the image to see the effect.</p>
<div class="container">
<img src="../assets/drink.jpg" alt="Avatar" class="image">
<div class="overlay">
<div class="text">Hello World</div>
</div>
</div>
</body>
</html>
```
### Table
```html
<!--Basic HTML Table Example-->
<!DOCTYPE html>
<html>
<head>
<style>
h2 {
text-align: center;
}

table {
border: 1px solid black;
}

th {
background-color: teal;
color: white;
padding: 5px;
}

td {
background-color: thistle;
text-align: center;
padding: 5px;
}

</style>
</head>
<body>
<h2>Our Menu</h2>
<table style="width:100%">
<tr>
<th>Breakfast</th>
<th>Lunch</th>
<th>Dinner</th>
</tr>
<tr>
<td>Eggs & Bacon</td>
<td>Pancakes & Sausage</td>
<td>Oatmeal & Fruit</td>
</tr>
<tr>
<td>Sanwiches</td>
<td>Soup</td>
<td>Salad</td>
</tr>
<tr>
<td>Steak & Potatos</td>
<td>Fried Chicken</td>
<td>Cheese Burger</td>
</tr>
</table>
</body>
</html>
```
### Text Over Image
```html
<!--TEXT OVER IMAGE EXAMPLE-->
<!DOCTYPE html>
<html>
<head>
<title>TEXT OVER IMAGE</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
/* Container holding the image and the text */
.container {
position: relative;
text-align: center;
color: white;
}

/* Bottom left text */
.bottom-left {
position: absolute;
bottom: 8px;
left: 16px;
}

/* Top left text */
.top-left {
position: absolute;
top: 8px;
left: 16px;
}

/* Top right text */
.top-right {
position: absolute;
top: 8px;
right: 16px;
}

/* Bottom right text */
.bottom-right {
position: absolute;
bottom: 8px;
right: 16px;
}

/* Centered text */

.centered {
position: absolute;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
}
</style>
</head>
<body>
<div class="container">
<img src="../assets/drink.jpg" alt="Snow" style="width:100%;">
<div class="bottom-left">From a company</div>
<div class="top-left">Wow this is cool</div>
<div class="top-right">It;s a drink</div>
<div class="bottom-right">that has bad marketing</div>
<div class="centered">With a name</div>
</div>
</body>
</html>
```
### Two Column Layout
```html
<!--TWO COLUMN LAYOUT-->
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
box-sizing: border-box;
}

.row {
display: flex;
}

/* Create two equal columns that sits next to each other */
.column {
flex: 50%;
padding: 10px;
height: 300px; /* Should be removed. Only for demonstration */
}
</style>
</head>
<body>
<h2>Two Equal Columns</h2>
<div class="row">
<div class="column" style="background-color:#aaa;">
<h2>Column 1</h2>
<p>Some text..</p>
</div>
<div class="column" style="background-color:#bbb;">
<h2>Column 2</h2>
<p>Some text..</p>
</div>
</div>
</body>
</html>
```
### Video Text Overlay
```html
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>

.container {
position: relative;
text-align: center;
color: white;
}

video {
width: 50%;
}

.centered {
position: absolute;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
font-size: large;
font-weight: bold;
}
</style>
</head>
<body>
<div class="container">
<video controls autoplay muted loop>
<source src="../assets/city.mp4" type="video/mp4">
</video>
<div class="centered">New York (maybe)</div>
</div>
</body>
</html>
```
### ViewPort Example
```html
<!--VIEWPORT EXAMPLE-->
<!DOCTYPE html>
<html>
<head>
<title>Viewport HTML</title>
<style>
@media screen and (max-width: 600px) {

p {
color:blue;
}

</style>
</head>
<body>
<p>Hello World</p>
</body>
</html>
```
