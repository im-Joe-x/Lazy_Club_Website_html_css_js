#  Lazy People Club - Multi Page Website

A fun and creative multi-page website developed using **HTML**, **CSS**, and **JavaScript** as part of a Web Technology project. The website is designed around the humorous concept of a **Lazy People Club**, providing an attractive user interface with interactive features and client-side form validation.

---
Html 
<!DOCTYPE html> 
<html> 
<head> 
<title>Lazy People Club</title> 
<link rel="stylesheet" href="proj4.css"> 
</head> 
<body> 
<header> 
<h1>        
<nav> 
Lazy People Club</h1> 
<a href="proj41.html">Home</a> 
<a href="proj42.html">Register</a> 
<a href="proj43.html">About</a> 
<a href="proj44.html">Gallery</a> 
<a href="proj45.html">Contact</a> 
</nav> 
</header> 
<section class="hero"> 
<h2>Welcome to the World's Laziest Club</h2> 
<p>If you love sleeping more than working, you belong here.</p> 
<a href="proj42.html"> 
<button class="join">Join the Lazy Club</button> 
</a> 
</section> 
</body> 
</html> 
<!DOCTYPE html> 
<html> 
<head> 
<title>Register</title> 
<link rel="stylesheet" href="proj4.css"> 
<script src="proj4.js"></script> 
</head> 
<body> 
<header> 
<h1>Lazy Club Registration</h1> 
</header> 
<div class="formbox"> 
<label>Name</label> 
<input type="text" id="name"> 
<label>Hours You Sleep</label> 
<input type="number" id="sleep"> 
<label>Laziness Level (1-10)</label> 
<input type="number" id="lazy"> 
<button onclick="checkForm()">Submit</button> 
<p id="message"></p> 
</div> 
</body> 
</html> 
<!DOCTYPE html> 
<html> 
<head> 
<title>About</title> 
<link rel="stylesheet" href="proj4.css"> 
</head> 
<body> 
<header> 
<h1>About Lazy Club</h1> 
</header> 
<div class="content"> 
<p> 
Lazy People Club is a community of people who believe 
sleeping is the best hobby. 
</p> 
<p> 
Our mission: 
Eat → Sleep → Repeat 
</p> 
</div> 
</body> 
</html> 
<!DOCTYPE html> 
<html> 
<head> 
<title>Lazy Gallery</title> 
<link rel="stylesheet" href="proj4.css"> 
</head> 
<body> 
<header> 
<h1>Lazy Moments Gallery</h1> 
</header> 
<div class="gallery"> 
<img src="lazy.jpg"> 
<img src="lazy1.jpg"> 
<img src="Depressed girl lying on sofa and looking at phone screen.jpg"> 
<img src="3776866.jpg"> 
</div> 
</body> 
</html> 
<!DOCTYPE html> 
<html> 
<head> 
<title>Lazy Gallery</title> 
<link rel="stylesheet" href="proj4.css"> 
</head> 
<body> 
<header> 
<h1>Lazy Moments Gallery</h1> 
</header> 
<div class="gallery"> 
<img src="lazy.jpg"> 
<img src="lazy1.jpg"> 
<img src="Depressed girl lying on sofa and looking at phone screen.jpg"> 
<img src="3776866.jpg"> 
</div> 
</body> 
</html> 
CSS 
body{ 
margin:0; 
font-family:Arial; 
color:white; 
text-align:center; 
background-image:url("6875483.jpg"); 
background-size:cover; 
background-attachment:fixed; 
} 
header{ 
background:rgba(0,0,0,0.6); 
padding:20px; 
} 
nav a{ 
color:white; 
margin:15px; 
text-decoration:none; 
font-size:18px; 
} 
nav a:hover{ 
color:yellow; 
} 
.hero{ 
margin-top:100px; 
} 
.join{ 
padding:15px 30px; 
font-size:18px; 
background:orange; 
border:none; 
border-radius:10px; 
cursor:pointer; 
} 
.join:hover{ 
background:red; 
} 
.formbox{ 
background:rgba(0,0,0,0.7); 
width:300px; 
margin:auto; 
padding:30px; 
border-radius:10px; 
} 
input{ 
width:100%; 
padding:10px; 
margin:10px 0; 
} 
button{ 
padding:10px 20px; 
background:green; 
border:none; 
color:white; 
cursor:pointer; 
} 
.gallery{ 
display:flex; 
justify-content:center; 
flex-wrap:wrap; 
gap:20px; 
padding:50px; 
} 
.gallery img{ 
border-radius:10px; 
width:300px; 
transition:0.4s; 
} 
.gallery img:hover{ 
transform:scale(1.1); 
} 
JS 
function checkForm(){ 
let name = document.getElementById("name").value; 
let sleep = document.getElementById("sleep").value; 
let lazy = document.getElementById("lazy").value; 
let msg = document.getElementById("message"); 
if(name == ""){ 
msg.textContent = "Even lazy people have names!"; 
return; 
} 
if(sleep < 6){ 
msg.textContent = "You need more sleep to join this club."; 
return; 
} 
if(lazy < 5){ 
msg.textContent = "You are too active for this club."; 
return; 
} 
msg.textContent = "Congratulations! You are officially lazy enough."; 
}


  
This project is created for educational purposes.
