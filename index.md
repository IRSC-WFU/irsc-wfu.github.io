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
  background-color: rgba(0,0,0,0.4);
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
  position: relative;
  bottom: 8px;
  width: auto;
  text-align: center;
  background-color: grey;
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
  background-color: grey;
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
  -webkit-animation-duration: 3s;
  animation-name: fade;
  animation-duration: 3s;
}

@-webkit-keyframes fade {
  from {opacity: .6} 
  to {opacity: 1}
}

@keyframes fade {
  from {opacity: .6} 
  to {opacity: 1}
}

/* On smaller screens, decrease text size */
@media only screen and (max-width: 300px) {
  .prev, .next,.text {font-size: 11px}
}

.slide-image{
    width:auto;
    height: 60vh;
    display: block;
    margin-left: auto;
    margin-right: auto;
}
</style>

<div class="slideshow-container">

<div class="mySlides fade">
  <a href="/members#faculty" style="text-decoration: none;">
    <div class="numbertext">1 / 4</div>
    <img class="slide-image" src="media/news/faculty-COLLAGE.jpg">
    <div class="text">Meet our faculty!</div>
  </a>
</div>

<div class="mySlides fade">
  <a href="/members#researchers" style="text-decoration: none;">
    <div class="numbertext">2 / 4</div>
    <img class="slide-image" src="media/news/researchers-COLLAGE.jpg">
    <div class="text">Meet our researchers!</div>
  </a>
</div>

<div class="mySlides fade">
  <a href="/members#student-research-team" style="text-decoration: none;">
    <div class="numbertext">3 / 4</div>
    <img class="slide-image" src="media/news/student-research-team-COLLAGE.jpg">
    <div class="text">Meet our student research team!</div>
  </a>
</div>

<div class="mySlides fade">
    <div class="numbertext">4 / 4</div>
    <img class="slide-image" src="media/news/LabGroupPhoto.jpeg">
    <div class="text">Our Summer Kick Off Social!</div>
</div>

<a class="prev" onclick="plusSlides(-1)">&#10094;</a>
<a class="next" onclick="plusSlides(1)">&#10095;</a>

</div>
<br>

<div style="text-align:center">
  <span class="dot" onclick="currentSlide(1)"></span> 
  <span class="dot" onclick="currentSlide(2)"></span> 
  <span class="dot" onclick="currentSlide(3)"></span>
  <span class="dot" onclick="currentSlide(4)"></span>
</div>

<script>
var slideIndex = 1;
var slideInterval = setInterval(plusSlides, 5000, 1);

showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}


function showSlides(n) {
  clearInterval(slideInterval);
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
  slideInterval = setInterval(plusSlides, 5000, 1);
}
</script>
<!--- End News Feed Slideshow --->

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
Coming Soon!


-------------------------
### [Publications](publications.md)
Here are some of the lab's recent publications!


- Ashley Peake, Joe McCalmon, Yixin Zhang, Daniel Myers, Sarra Alqahtani, Victor Paúl Pauca, "Deep Reinforcement Learning for Adaptive Exploration of Unknown Environments", the IEEE International Conference on Unmanned Aircraft Systems, (ICUAS '21).

- Yixin Zhang, Joe McCalmon, Ashley Peake, Sarra Alqahtani, Victor Paúl Pauca, "A Symbolic-AI Approach for UAV Exploration Tasks", the 8th International Conference on Automation, Robotics and Applications (ICARA 2021), accepted.

- Xiaotian Liu, Pengyi Shi, TongTong Liu, Sarra Alqahtani, Victor Paúl Pauca, and Miles Silman, "Robustness-Driven Exploration with Probabilistic Metric Temporal Logic", the 13th International Conference on Agents and Artificial Intelligence (ICAART 2021).

- Ashley Peake\*, Joe McCalmon\*, Yixin Zhang, Benjamin Raiford, and Sarra Alqahtani, "Wilderness Search and Rescue Missions using Deep Reinforcement Learning," IEEE International Symposium on Safety, Security, and Rescue Robotics (SSRR), 2020.

- Camalan, S.; Cui, K.; Pauca, V.P.; Alqahtani, S.; Silman, M.; Chan, R.; Plemmons, R.J.; Dethier, E.N.; Fernandez, L.E.; Lutz, D.A. Change Detection of Amazonian Alluvial Gold Mining Using Deep Learning and Sentinel-2 Imagery. Remote Sens. 2022, 14, 1746. https://doi.org/10.3390/rs14071746


-------------------------
### [Contact](contact.md)
Coming Soon!
