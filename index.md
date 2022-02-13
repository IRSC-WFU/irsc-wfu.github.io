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
    <div class="numbertext">1 / 3</div>
    <img class="slide-image" src="media/news/faculty-COLLAGE.jpg">
    <div class="text">Meet our faculty!</div>
  </a>
</div>

<div class="mySlides fade">
  <a href="/members#researchers" style="text-decoration: none;">
    <div class="numbertext">2 / 3</div>
    <img class="slide-image" src="media/news/researchers-COLLAGE.jpg">
    <div class="text">Meet our researchers!</div>
  </a>
</div>

<div class="mySlides fade">
  <a href="/members#student-research-team" style="text-decoration: none;">
    <div class="numbertext">3 / 3</div>
    <img class="slide-image" src="media/news/student-research-team-COLLAGE.jpg">
    <div class="text">Meet our student research team!</div>
  </a>
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
### [Members](members.md)
#### Faculty
<style>
.card-body{
    min-height:100vh;
    display: flex;
    justify-content: center;
    align-items: center;
}
.card-wrapper{
    width:100%;
    height:100%;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover; 
}
.card-wrapper .card-box{
    position: relative;
    width:280px;
    height:400px;
    border-radius:15px;
    margin:30px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-top:1px solid rgba(255,255,255,0.5);
    border-left:1px solid rgba(255,255,255,0.5);
}
.card-box{
    background-image: linear-gradient(120deg, #155799, #159957);
    box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
    
}
.description {
    text-align: center;
}
.description h2{
    color:#f5f5f5;
    font-size:2rem;
    text-align: center;
    font-family: 'Acme', sans-serif;
}
.description p{
    color:#ccc;
    margin:20px 10px;
    font-family: 'Fira Code', monospace;
    font-size: 1rem;
}
.image-cropper {
  width: auto;
  height: 120px;
  position: relative;
  overflow: hidden;
}
.image-cropper img {
    max-height: -webkit-fill-available;
    border-radius: 50%;
}
.card-link:hover{
    text-decoration: none;
}
.card-box:hover{
    box-shadow: 0 4px 8px 0 rgba(0,0,0,0.4);
    transition: 0.3s;
}
</style>

<div class="card-wrapper">
    <div class="card-box">
        <a class="card-link" href="/members/sarra_alqahtani">
            <div class="description">
                <div class="image-cropper">
                    <img src="/media/members/Alqahtani.jpg" height="120px"/>
                </div>
                <h2>Sarra Alqahtani</h2>
                <p>Assistant Professor</p>
                <p>Department of Computer Science</p>
                <p>Wake Forest University</p>
            </div>
        </a>
    </div>
    <div class="card-box">
        <a class="card-link" href="/members/paul_pauca">
            <div class="description">
                <div class="image-cropper">
                    <img src="/media/members/Paul2.jpg" height="120px"/>
                </div>
                <h2>Paúl Pauca</h2>
                <p>Professor</p>
                <p>Department of Computer Science</p>
                <p>Wake Forest University</p>
            </div>
        </a>
    </div>
    <div class="card-box">
        <a class="card-link" href="/members/miles_silman">
            <div class="description">
                <div class="image-cropper">
                    <img src="/media/members/silman.jpg" height="120px"/>
                </div>
                <h2>Miles Silman</h2>
                <p>Professor</p>
                <p>Department of Biology</p>
                <p>Wake Forest University</p>
            </div>
        </a>
    </div>
    <div class="card-box">
        <a class="card-link" href="/members/luis_fernandez">
            <div class="description">
                <div class="image-cropper">
                    <img src="/media/members/Luis.jpg" height="120px"/>
                </div>
                <h2>Luis E. Fernandez</h2>
                <p>Executive Director</p>
                <p>Amazonian Scientific Innovation</p>
                <p>Wake Forest University</p>
            </div>
        </a>
    </div>
    <div class="card-box">
        <a class="card-link" href="/members/david_lutz">
            <div class="description">
                <div class="image-cropper">
                    <img src="/media/members/david_lutz.jpg" height="120px"/>
                </div>
                <h2>David A. Lutz</h2>
                <p>Research Assistant Professor</p>
                <p>Department of Environmental Studies</p>
                <p>Dartmouth College</p>
            </div>
        </a>
    </div>
    <div class="card-box">
        <a class="card-link" href="/members/bob_plemmons">
            <div class="description">
                <div class="image-cropper">
                    <img src="/media/members/bob_plemmons.jpg" height="120px"/>
                </div>
                <h2>Bob Plemmons</h2>
                <p>Research Professor</p>
                <p>Departments of Computer Science and Mathematics</p>
                <p>Wake Forest University</p>
            </div>
        </a>
    </div>
</div>

#### Researchers
<div class="card-wrapper">
    <div class="card-box">
        <a class="card-link" href="/members/seda_camalan">
            <div class="description">
                <div class="image-cropper">
                    <img src="/media/members/Seda-Camalan.jpg" height="120px"/>
                </div>
                <h2>Seda Camalan</h2>
                <p>Postdoctoral Fellow</p>
                <p>Department of Computer Science</p>
                <p>Wake Forest University</p>
            </div>
        </a>
    </div>
    <div class="card-box">
        <a class="card-link" href="/members/evan_dethier">
            <div class="description">
                <div class="image-cropper">
                    <img src="/media/members/evan new.jpg" height="120px"/>
                </div>
                <h2>Evan Dethier</h2>
                <p>Postdoctoral Fellow</p>
                <p>Department of Earth Sciences</p>
                <p>Dartmouth College</p>
            </div>
        </a>
    </div>
    <div class="card-box">
        <a class="card-link" href="/members/jason_cui">
            <div class="description">
                <div class="image-cropper">
                    <img src="/media/members/kcui.jpg" height="120px"/>
                </div>
                <h2>Jason Cui</h2>
                <p>Researcher</p>
                <p>Department of Mathematics</p>
                <p>City University of Hong Kong</p>
            </div>
        </a>
    </div>
    <div class="card-box">
        <a class="card-link" href="/members/robert_langefeld">
            <div class="description">
                <div class="image-cropper">
                    <img src="/media/members/robert_langefeld.jpg" height="120px"/>
                </div>
                <h2>Robert Langefeld</h2>
                <p>Researcher</p>
                <p>Departments of Mathematics and Computer Science</p>
                <p>Wake Forest University</p>
            </div>
        </a>
    </div>
</div>

#### Student Research Team
<div class="card-wrapper">
    <div class="card-box">
        <a class="card-link" href="/members/adelina_sederman">
            <div class="description">
                <div class="image-cropper">
                    <img src="/media/members/adelina_sederman.jpg" height="120px"/>
                </div>
                <h2>Adelina Sederman</h2>
                <p>Research Assistant</p>
                <p>Department of Engineering Sciences and Environmental Sciences</p>
                <p>Dartmouth College</p>
            </div>
        </a>
    </div>
    <div class="card-box">
        <a class="card-link" href="/members/isaias_bahena">
            <div class="description">
                <div class="image-cropper">
                    <img src="/media/members/isaias_bahena.jpg" height="120px"/>
                </div>
                <h2>Isaias Bahena</h2>
                <p>Research Assistant</p>
                <p>Department of Computer Science</p>
                <p>Wake Forest University</p>
            </div>
        </a>
    </div>
    <div class="card-box">
        <a class="card-link" href="/members/daniel_langefeld">
            <div class="description">
                <div class="image-cropper">
                    <img src="/media/members/daniel_langefeld.jpg" height="120px"/>
                </div>
                <h2>Daniel Langefeld</h2>
                <p>Research Assistant</p>
                <p>High School Senior</p>
                <p>Wesleyan Christian Academy</p>
            </div>
        </a>
    </div>
    <div class="card-box">
        <a class="card-link" href="/members/alice_li">
            <div class="description">
                <div class="image-cropper">
                    <img src="/media/members/alice_li.jpg" height="120px"/>
                </div>
                <h2>Alice Li</h2>
                <p>Research Assistant</p>
                <p>Departments of Statistics and Computer Science</p>
                <p>Wake Forest University</p>
            </div>
        </a>
    </div>
    <div class="card-box">
        <a class="card-link" href="/members/shanyu_gowdu">
            <div class="description">
                <div class="image-cropper">
                    <img src="/media/members/shanyu_gowdu.jpg" height="120px"/>
                </div>
                <h2>Shanyu Gowdu</h2>
                <p>Research Assistant</p>
                <p>High School Junior</p>
                <p>North Carolina School of Science and Math</p>
            </div>
        </a>
    </div>
</div>


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



-------------------------
### [Contact](contact.md)
Coming Soon!
