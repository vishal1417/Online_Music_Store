# Online_Music_Store


<!DOCTYPE html>
<html>
<head>
<link rel="shortcut icon" href="images/title_logo.ico" />
<title>Online Music Store</title>
<link href="css/index.css" rel="stylesheet" type="text/css" />
<link href="css/nav.css" rel="stylesheet" type="text/css" />
<link href="css/footer.css" rel="stylesheet" type="text/css" />
<link href="css/modal.css" rel="stylesheet" type="text/css" />
</head>
<body>
<div class="modal">
<span class="close" >&times;</span>
<div class="modal-content">
<form method="post">
<div class="log">
<h1>LOGIN</h1>
<input class="username" type="text" placeholder="Username" required name="username">
<br/>
<input class="password" type="password" placeholder="Password" required name="password">
<br/>
<button type="submit">LOG IN</button>
<p>Forgot <a href="#">Password ?</a></p>
</div>
</form>
<div class="sign">
<form method="post">
<h1>SIGN UP</h1>
<input class="username" type="text" placeholder="Username" required name="username">
<br/>
<input class="password" type="password" placeholder="Password" required name="password">
<br/>
<input class="password" type="password" placeholder="Re-Enter Password" required name="password">
<br/>
<button type="submit">SIGN UP</button>
</div>
</form>
</div>
</div>
<header>
<div class="navigation">
<img src="images/logo.png" height=77 width=87 class="logo" />
<nav>
<ul>
<li><a href="index.html" id="on">home</a></li>
<li><a href="html/english.html">English</a></li>
<li><a href="html/hindi.html">Hindi</a></li>
<li><a href="#c">Contact Us</a></li>
<li><a href="#" id="login">Login/Register</a></li>
<li><a href="#"><img src="images/search.png" width=35 height=35 alt="search logo" class="logo1" /></a></li>
</ul>
</nav>
</div>
</header>
<div class="slideshow_container">
<div class="mySlides">
<img src="images/1.jpg" width=100% />
<div class="context">Music That Suits Your Needs</div>
</div>
<div class="mySlides">
<img src="images/2.jpg" width=100% />
<div class="context">High Quality Music</div>
</div>
<div class="mySlides">
<img src="images/3.jpg" width=100% />
<div class="context">Music For Everyone</div>
</div>
<div class="mySlides">
<img src="images/4.jpg" width=100% />
<div class="context">Latest And Exclusive Content</div>
</div>
</div>
<div class="white_container">
<h1>Online Music Store</h1>
<p id="fade">We love Music</p>
<p id="info">You???ll find almost any type of audio content you???re in the mood for! We have an enormous collection of 
both international as well as Indian music spanning multiple genres and languages. 
You???ll find everything from the music of the 50???s to the latest hits. Wait, it gets better! We also have exclusive album releases on Store! 
Yes, you???ll be the first to get access to these exclusive releases.
</div>
<div class="black_container">
<h1>The best music experience, only better.</h1>
<div class="logo2">
<img src="images/download_logo.png" />
<div class="description">Save Data, Listen Offline</div>
</div>
<div class="logo2">
<img src="images/high_quality.png" />
<div class="description">Beautiful 320kbps Audio</div>
</div>
<div class="logo2">
<img src="images/exclusive.png" />
<div class="description" id="fault1">Access Exclusive Content</div>
</div>
</div>
</div>
<div class="contact" id="c">
<h1>CONTACT US</h1>
<p id="fade_contact">Fan? Drop a note!</p>
<div class="contact1">
<div class="contact_details">
<img src="images/ping.png" width=25px />
<div class="details">Jalandhar, India</div>
</div>
<div class="contact_details">
<img src="images/call.png" width=25px />
<div class="details">Phone: +91 181-765432</div>
</div>
<div class="contact_details">
<img src="images/email.png" width=25px />
<div class="details">Email: OMS@mail.com</div>
</div>
</div>
<div class="contact_form">
<form method="post">
<div>
<input class="name" type="text" placeholder="Name" required name="Name">
<input class="email" type="text" placeholder="Email" required name="Email">
</div>
<div>
<input class="message" type="text" placeholder="Message" required name="Message">
</div>
<button class="send" type="submit">SEND</button>
</form>
</div>
</div>
<div class="grey_container">
<a href="#"><img src="images/social.png" width=17%></a>
<p>Powered By HTML &amp; CSS.</p>
<p>Copyright &copy; 2017 OMS. All rights reserved.</p>
</div>
<script src="js/slideshow.js"></script>
<script src="js/modal.js"></script>
</body>
</html>
====================================================================
js for model


document.addEventListener('play', function(e){
    var allAudios = document.getElementsByTagName('audio');
    for(var i = 0; i<allAudios.length; i++){
        if(allAudios[i] != e.target){
            allAudios[i].pause();
        }
    }
}, true);

====================================
js  for audio


document.addEventListener('play', function(e){
    var allAudios = document.getElementsByTagName('audio');
    for(var i = 0; i<allAudios.length; i++){
        if(allAudios[i] != e.target){
            allAudios[i].pause();
        }
    }
}, true);
===============================
=======
js for slideshow




var myIndex = 0;
carousel();

function carousel() {
    var i;
    var x = document.getElementsByClassName("mySlides");
    for (i = 0; i < x.length; i++) {
       x[i].style.display = "none";  
    }
    myIndex++;
    if (myIndex > x.length) {myIndex = 1}    
    x[myIndex-1].style.display = "block";  
    setTimeout(carousel, 2000); // Change image every 2 seconds
}
