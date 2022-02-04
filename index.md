---
layout: default
title: Home
navigation_weight: 1
---

## Wake Forest IRSC Lab

Wake Forest's Intelligent Remote Sensing in Conservation & Discovery Group (IRSC Lab) is an interdisciplinary group of researchers from Wake Forest's Biology and Computer Science departments in collaboration with researchers and conservationists at Dartmouth College and [The Center for Amazonian Scientific Innovation](https://cincia.wfu.edu/en/) in Peru. Our lab works on methods to apply machine learning, artificial intelligence, and statistics to the problems of conservation in the Peruvian Amazon and around the world.

-------------------------
### [News](news.md)

<!--- Begin News Feed Slideshow --->
<style>
* {box-sizing: border-box}
body {font-family: Verdana, sans-serif; margin:0}
.mySlides {display: none}
img {vertical-align: middle;}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}

/* Next & previous buttons */
.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  padding: 16px;
  margin-top: -22px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6s ease;
  border-radius: 0 3px 3px 0;
  user-select: none;
}

/* Position the "next button" to the right */
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover, .next:hover {
  background-color: rgba(0,0,0,0.8);
}

/* Caption text */
.text {
  color: #f2f2f2;
  font-size: 15px;
  padding: 8px 12px;
  position: absolute;
  bottom: 8px;
  width: 100%;
  text-align: center;
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* The dots/bullets/indicators */
.dot {
  cursor: pointer;
  height: 15px;
  width: 15px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.active, .dot:hover {
  background-color: #717171;
}

/* Fading animation */
.fade {
  -webkit-animation-name: fade;
  -webkit-animation-duration: 1.5s;
  animation-name: fade;
  animation-duration: 1.5s;
}

@-webkit-keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

@keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

/* On smaller screens, decrease text size */
@media only screen and (max-width: 300px) {
  .prev, .next,.text {font-size: 11px}
}
</style>

<div class="slideshow-container">

<div class="mySlides fade">
  <div class="numbertext">1 / 3</div>
  <img src="media/test_puppy.jpg" style="width:100%">
  <div class="text">Caption Text</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">2 / 3</div>
  <img src="media/test_puppy.jpg" style="width:100%">
  <div class="text">Caption Two</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">3 / 3</div>
  <img src="media/test_puppy.jpg" style="width:100%">
  <div class="text">Caption Three</div>
</div>

<a class="prev" onclick="plusSlides(-1)">&#10094;</a>
<a class="next" onclick="plusSlides(1)">&#10095;</a>

</div>
<br>

<div style="text-align:center">
  <span class="dot" onclick="currentSlide(1)"></span> 
  <span class="dot" onclick="currentSlide(2)"></span> 
  <span class="dot" onclick="currentSlide(3)"></span> 
</div>

<script>
var slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  var i;
  var slides = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("dot");
  if (n > slides.length) {slideIndex = 1}    
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";  
  }
  for (i = 0; i < dots.length; i++) {
      dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";  
  dots[slideIndex-1].className += " active";
}
</script>
<!--- End News Feed Slideshow --->

-------------------------
### [Members](members.md)
#### Faculty
<style>
*{
    margin:0;
    padding:0;
    box-sizing: border-box;
}
.card-body{
    min-height:100vh;
    display: flex;
    justify-content: center;
    align-items: center;
}
.card-wrapper{
    width:100%;
    height:100%;
    min-height: 100vh;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    background-image: url("https://images.pexels.com/photos/3503629/pexels-photo-3503629.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940");
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover; 
}
.card-wrapper .card-box{
    position: relative;
    width:280px;
    height:400px;
    box-shadow: 20px 20px 50px rgba(0,0,0,0.5);
    border-radius:15px;
    margin:30px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-top:1px solid rgba(255,255,255,0.5);
    border-left:1px solid rgba(255,255,255,0.5);
    backdrop-filter: blur(5px);
    transform-style: preserve-3d;
    transform: perspective(800px) 
}
.description h2{
    color:#f5f5f5;
    font-size:2.5rem;
    text-align: center;
    font-family: 'Acme', sans-serif;
}
.description p{
    color:#ccc;
    margin:20px 10px;
    font-family: 'Fira Code', monospace;
}
.description ul{
    list-style: none;
    width:100%;
    display: flex;
    justify-content: space-evenly;
    margin:30px 0;
    padding:10px;
}

ul.list li{
    cursor: pointer;
    width:30px;
    height:30px;
}
i{
    color:#ccc;
    font-size: 1.5rem;
    transition: all 0.3s ease;
}
ul.list li:hover .fa-twitter{
    transform:translate3d(0,-10px,20px);
    color:#00acee;
}
ul.list li:hover .fa-github{
    transform:translate3d(0,-10px,20px);
    color:gray;
}
ul.list li:hover .fa-linkedin-in{
    transform:translate3d(0,-10px,20px);
    color:#077099;
}
</style>

<script>
 VanillaTilt.init(document.querySelectorAll(".box"), {
		max: 25,
        speed: 400,
        easing:"cubic-bezier(.03,.98,.52,.99)",
        perspective:500,
        transition:true
    });
</script>

<div class="card-wrapper">
    <div class="card-box">
        <div class="description">
            <h2><a href="/members/sarra_alqahtani">Sarra Alqahtani</a></h2>
            <p>Assistant Professor</p>
            <p>Department of Computer Science</p>
            <p>Wake Forest University</p>
            <img src="/media/members/Alqahtani.png"/>
            <ul class="list">
                <li><a href="https://github.com/rlangefe"><i class="fab fa-github"></i></a></li>
            </ul>
        </div>
    </div>
</div>

<style>
.card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  width: 20%;
  border-radius: 5px;
}

.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}

.card img {
  border-radius: 5px 5px 0 0;
}

.caption h3,p {
    text-align: center
    font-size: 16em;
}

.card-container {
  padding: 2px 16px;
}
</style>

<div class="member-table">
    <div class="card">
        <div class="img">
            <img src="/media/members/Alqahtani.png"/>
        </div>
        <div class="caption">
            <h3><a href="/members/sarra_alqahtani">Sarra Alqahtani</a></h3>
            <p>Assistant Professor</p>
            <p>Department of Computer Science</p>
            <p>Wake Forest University</p>
        </div>
    </div>
    <div class="card">
        <div class="img">
            <img src="/media/members/Paul2.jpg"/>
        </div>
        <div class="caption">
            <h3><a href="/members/paul_pauca">Paúl Pauca</a></h3>
            <p>Professor</p>
            <p>Department of Computer Science</p>
            <p>Wake Forest University</p>
        </div>
    </div>
    <div class="card">
        <div class="img">
            <img src="/media/members/silman.jpg"/>
        </div>
        <div class="caption">
            <h3><a href="/members/miles_silman">Miles Silman</a></h3>
            <p>Professor</p>
            <p>Department of Biology</p>
            <p>Wake Forest University</p>
        </div>
    </div>
    <div class="card">
        <div class="img">
            <img src="/media/members/Luis.jpg"/>
        </div>
        <div class="caption">
            <h3><a href="/members/luis_fernandez">Luis E. Fernandez</a></h3>
            <p>Executive Director</p>
            <p>Amazonian Scientific Innovation</p>
            <p>Wake Forest University</p>
        </div>
    </div>
    <div class="card">
        <div class="img">
            <img src="/media/members/david_lutz.jpg"/>
        </div>
        <div class="caption">
            <h3><a href="/members/david_lutz">David A. Lutz</a></h3>
            <p>Research Assistant Professor</p>
            <p>Department of Environmental Studies</p>
            <p>Dartmouth College</p>
        </div>
    </div>     
</div>

#### Researchers
<div class="member-table">
    <div class="flip-card">
        <div class="flip-card-inner">
            <div class="flip-card-front">
                <img class="member-img" src="/media/members/Seda-Camalan.jpg" alt="1" width = 200px height = 200px >
            </div>
        <div class="flip-card-back">
            <h2><a href="/members/seda_camalan">Seda Camalan</a></h2>
            <p>Postdoctoral Fellow</p>
            <p>Department of Computer Science</p>
            <p>Wake Forest University</p>
            </div>
        </div>
    </div>
    <div class="flip-card">
        <div class="flip-card-inner">
            <div class="flip-card-front">
                <img class="member-img" src="/media/members/evan new.jpg" alt="1" width = 200px height = 200px >
            </div>
        <div class="flip-card-back">
            <h2><a href="/members/evan_dethier">Evan Dethier</a></h2>
            <p>Postdoctoral Fellow</p>
            <p>Department of Earth Sciences</p>
            <p>Dartmouth College</p>
            </div>
        </div>
    </div>
    <div class="flip-card">
        <div class="flip-card-inner">
            <div class="flip-card-front">
                <img class="member-img" src="/media/members/robert_langefeld.jpg" alt="1" width = 200px height = 200px >
            </div>
        <div class="flip-card-back">
            <h2><a href="/members/robert_langefeld">Robert Langefeld</a></h2>
            <p>Researcher</p>
            <p>Departments of Mathematics and Computer Science</p>
            <p>Wake Forest University</p>
            </div>
        </div>
    </div>
</div>

#### Student Research Team
<div class="member-table">
    <div class="flip-card">
        <div class="flip-card-inner">
            <div class="flip-card-front">
                <img class="member-img" src="/media/members/adelina_sederman.jpg" alt="1" width = 200px height = 200px >
            </div>
        <div class="flip-card-back">
            <h2><a href="/members/adelina_sederman">Adelina Sederman</a></h2>
            <p>Research Assistant</p>
            <p>Department of Engineering Sciences and Environmental Sciences</p>
            <p>Dartmouth College</p>
            </div>
        </div>
    </div>
    <div class="flip-card">
        <div class="flip-card-inner">
            <div class="flip-card-front">
                <img class="member-img" src="/media/members/isaias_bahena.jpg" alt="1" width = 200px height = 200px >
            </div>
        <div class="flip-card-back">
            <h2><a href="/members/isaias_bahena">Isaias Bahena</a></h2>
            <p>Research Assistant</p>
            <p>Department of Computer Science</p>
            <p>Wake Forest University</p>
            </div>
        </div>
    </div>
    <div class="flip-card">
        <div class="flip-card-inner">
            <div class="flip-card-front">
                <img class="member-img" src="/media/members/daniel_langefeld.jpg" alt="1" width = 200px height = 200px >
            </div>
        <div class="flip-card-back">
            <h2><a href="/members/daniel_langefeld">Daniel Langefeld</a></h2>
            <p>Research Assistant</p>
            <p>High School Senior</p>
            <p>Wesleyan Christian Academy</p>
            </div>
        </div>
    </div>
    <div class="flip-card">
        <div class="flip-card-inner">
            <div class="flip-card-front">
                <img class="member-img" src="/media/members/alice_li.jpg" alt="1" width = 200px height = 200px >
            </div>
        <div class="flip-card-back">
            <h2><a href="/members/alice_li">Alice Li</a></h2>
            <p>Research Assistant</p>
            <p>Departments of Statistics and Computer Science</p>
            <p>Wake Forest University</p>
            </div>
        </div>
    </div>
    <div class="flip-card">
        <div class="flip-card-inner">
            <div class="flip-card-front">
                <img class="member-img" src="/media/test_puppy.jpg" alt="1" width = 200px height = 200px >
            </div>
        <div class="flip-card-back">
            <h1>John Doe</h1>
            <p>Architect & Engineer</p>
            <p>We love that guy</p>
            </div>
        </div>
    </div>
    <div class="flip-card">
        <div class="flip-card-inner">
            <div class="flip-card-front">
                <img class="member-img" src="/media/test_puppy.jpg" alt="1" width = 200px height = 200px >
            </div>
        <div class="flip-card-back">
            <h1>John Doe</h1>
            <p>Architect & Engineer</p>
            <p>We love that guy</p>
            </div>
        </div>
    </div>        
</div>

<style>
.member-img {
  border-radius: 10%;
  object-fit: cover;
}

.member-table {
    width: 100%;
    display: flex;
    flex-flow: row wrap;
    justify-content: center;
    margin-left: auto;
    margin-right: auto;
    row-gap: 10px;
    column-gap: 10px;
}

/* The flip card container - set the width and height to whatever you want. We have added the border property to demonstrate that the flip itself goes out of the box on hover (remove perspective if you don't want the 3D effect */
.flip-card {
  background-color: transparent;
  width: 200px;
  height: 200px;
  perspective: 1000px; /* Remove this if you don't want the 3D effect */
}

/* This container is needed to position the front and back side */
.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.8s;
  transform-style: preserve-3d;
}

/* Do an horizontal flip when you move the mouse over the flip box container */
.flip-card:hover .flip-card-inner {
  transform: rotateY(180deg);
}

/* Position the front and back side */
.flip-card-front, .flip-card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  -webkit-backface-visibility: hidden; /* Safari */
  backface-visibility: hidden;
}

/* Style the front side (fallback if image is missing) */
.flip-card-front {
  color: black;
}

/* Style the back side */
.flip-card-back {
  background-color: grey;
  color: white;
  transform: rotateY(180deg);
  border-radius: 10%;
  display: block;
  font-size: 1.1vh;
}
</style>


-------------------------
### [Research](research.md)
Our lab explores novel methods and applications for computational technology to the fields of conservation and ecology. We explore questions such as

* Accurate satellite and drone image segmentation
* Large-scale object identification
* Time series analyses of mining regions
    * Change detection
    * Predicting new mining activity


* Data fusion techniques
    * Methods for combining data from different sources
    * Methods for generalizing models to different sources

* Statistical analyses of regions
    * Object significance
    * Relationships with environmental significance

* High performance computing solutions
    * Methods that leverage computation for better results
    * Efficient methods that are accessible and open source for researchers without a computer science background


* Software development
    * Software design to integrate machine learning models and predictions


-------------------------
### [Projects](projects.md)
Featured projects


-------------------------
### [Publications](publications.md)
Featured publications


-------------------------
### [Contact](contact.md)
Contact info
