---
layout: post
title: "Anonymous Sorrow - Ann Marie Stillion"
author: "Deana Seitz and Aster Teter"
categories: gallery
tags: [gallery, color grading, editing]
image: as-1.jpg
---

<style>
@import url("https://fonts.googleapis.com/css?family=Rozha+One");
@import url("https://fonts.googleapis.com/css?family=Raleway|Rozha+One");

body {
  background-color: #a4a4a4;
}
.col4 {
  width: 33.33333333%;
  float: left;
  position: relative;
}
.transition {
  -webkit-transition: all 0.5s ease;
  -moz-transition: all 0.5s ease;
  -o-transition: all 0.5s ease;
  transition: all 0.5s ease;
}
body .container {
  width: 70%;
  margin: 0 auto;
}
.fx1 .item,
.fx2 .item,
.fx3 .item,
.fx4 .item,
.fx5 .item {
  margin: 10px 0;
}

/* active on focus for accessibility tab navigation */

.fx1 .item {
  padding: 0;
}
.fx1 .item img {
  padding: 0 !important;
  display: block;
  max-width: 100%;
  height: auto;
}
.fx1 a:hover .item img,
.fx1 a:focus .item img {
  opacity: 0.8;
}
.fx1 h4,
.fx1 p {
  -webkit-transition: all 0.5s ease;
  -moz-transition: all 0.5s ease;
  -o-transition: all 0.5s ease;
  transition: all 0.5s ease;
}
.fx1 a .item h4 {
  font-family: "Raleway", sans-serif;
  font-size: 16px;
  position: absolute;
  color: #fff;
  text-transform: uppercase;
  letter-spacing: 2px;
  position: absolute;
  top: 42%;
  left: 0;
  right: 0;
  margin: 0 auto;
  text-align: center;
  opacity: 0;
}
.fx1 a:hover .item h4,
.fx1 a:focus .item h4 {
  opacity: 1;
}
.fx1 a .item p {
  font-family: "Raleway", sans-serif;
  font-size: 8px;
  position: absolute;
  color: #fff;
  text-transform: uppercase;
  letter-spacing: 2px;
  position: absolute;
  top: 52%;
  left: 0;
  right: 0;
  margin: 0 auto;
  text-align: center;
  opacity: 0;
}
.fx1 a:hover .item p,
.fx1 a:focus .item p {
  opacity: 1;
}

.fx2 .item {
  padding: 0;
}
.fx2 .item img {
  padding: 0 !important;
  display: block;
  max-width: 100%;
  height: auto;
}
.fx2 a:hover .item img,
.fx2 a:focus .item img {
  opacity: 0.9;
  -webkit-transform: scale(0.95);
  transform: scale(0.95);
}
.fx2 h4,
.fx2 p,
.fx2 span {
  -webkit-transition: all 0.5s ease;
  -moz-transition: all 0.5s ease;
  -o-transition: all 0.5s ease;
  transition: all 0.5s ease;
}
.fx2 a .item h4 {
  font-family: "Raleway", sans-serif;
  font-size: 16px;
  position: absolute;
  color: #fff;
  text-transform: uppercase;
  letter-spacing: 2px;
  position: absolute;
  top: 42%;
  left: 0;
  right: 0;
  margin: 0 auto;
  text-align: center;
  -webkit-filter: blur(5px);
  filter: blur(5px);
  opacity: 0;
}
.fx2 a:hover .item h4,
.fx2 a:focus .item h4 {
  -webkit-filter: blur(0px);
  filter: blur(0px);
  opacity: 1;
}
.fx2 a .item p {
  font-family: "Raleway", sans-serif;
  font-size: 8px;
  position: absolute;
  color: #fff;
  text-transform: uppercase;
  letter-spacing: 2px;
  position: absolute;
  top: 53%;
  left: 0;
  right: 0;
  margin: 0 auto;
  text-align: center;
  opacity: 0;
}
.fx2 a:hover .item p,
.fx2 a:focus .item p {
  opacity: 1;
}

.fx3 .item {
  padding: 0;
}
.fx3 .item img {
  padding: 0 !important;
  display: block;
  max-width: 100%;
  height: auto;
  outline: transparent solid 2px;
  outline-offset: 0px;
}
.fx3 a:hover .item img,
.fx3 a:focus .item img {
  opacity: 0.8;
  outline: #fff solid 2px;
  outline-offset: -10px;
}
.fx3 h4,
.fx3 p {
  -webkit-transition: all 0.5s ease;
  -moz-transition: all 0.5s ease;
  -o-transition: all 0.5s ease;
  transition: all 0.5s ease;
}
.fx3 a .item h4 {
  font-family: "Raleway", sans-serif;
  font-size: 16px;
  position: absolute;
  color: #fff;
  text-transform: uppercase;
  letter-spacing: 2px;
  position: absolute;
  top: 42%;
  left: 0;
  right: 0;
  margin: 0 auto;
  text-align: center;
  opacity: 0;
}
.fx3 a:hover .item h4,
.fx3 a:focus .item h4 {
  opacity: 1;
}
.fx3 a .item p {
  font-family: "Raleway", sans-serif;
  font-size: 8px;
  position: absolute;
  color: #fff;
  text-transform: uppercase;
  letter-spacing: 2px;
  position: absolute;
  top: 52%;
  left: 0;
  right: 0;
  margin: 0 auto;
  text-align: center;
  opacity: 0;
}
.fx3 a:hover .item p,
.fx3 a:focus .item p {
  opacity: 1;
}

.fx5 .item {
  padding: 0;
}
.fx5 .item img {
  padding: 0 !important;
  display: block;
  max-width: 100%;
  height: auto;
}
.fx5 a:hover .item img,
.fx5 a:focus .item img {
  opacity: 0.8;
}
.fx5 h4,
.fx5 p {
  -webkit-transition: all 0.5s ease-out;
  -moz-transition: all 0.5s ease-out;
  -o-transition: all 0.5s ease-out;
  transition: all 0.5s ease-out;
}
.fx5 a .item h4 {
  font-family: "Raleway", sans-serif;
  font-size: 16px;
  position: absolute;
  color: #fff;
  text-transform: uppercase;
  letter-spacing: 2px;
  background-color: #b5b5b5;
  padding: 5px 10px;
  position: absolute;
  bottom: 10%;
  left: 0%;
  opacity: 0;
}
.fx5 a:hover .item h4,
.fx5 a:focus .item h4 {
  opacity: 1;
  left: 10%;
}
.fx5 a .item p {
  font-family: "Raleway", sans-serif;
  font-size: 8px;
  position: absolute;
  color: #fff;
  text-transform: uppercase;
  letter-spacing: 2px;
  background-color: #b5b5b5;
  padding: 5px 10px;
  position: absolute;
  bottom: 7%;
  left: 0%;
  opacity: 0;
}
.fx5 a:hover .item p,
.fx5 a:focus .item p {
  opacity: 1;
  left: 10%;
}

@media screen and (max-width: 991px) {
  .col4 {
    width: 50%;
  }
  .fx5 a .item h4 {
    font-size: 13px;
  }
}

@media screen and (max-width: 580px) {
  .col4 {
    width: 100%;
  }
}

</style>

<div class="container">
<div class="container">
        
        <div class="fx1">

            <a href="#">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.unsplash.com/photo-1461611034385-e082102d5c75?auto=format&fit=crop&w=1050&q=60&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D">
                    <h4>title image</h4>
                    <p>Description</p>
                </div>
            </a>
            <a href="#">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.unsplash.com/photo-1461611034385-e082102d5c75?auto=format&fit=crop&w=1050&q=60&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D">
                    <h4>title image</h4>
                    <p>Description</p>
                </div>
            </a>
            <a href="#">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.unsplash.com/photo-1461611034385-e082102d5c75?auto=format&fit=crop&w=1050&q=60&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D">
                    <h4>title image</h4>
                    <p>Description</p>
                </div>
            </a>
            
        </div>  
        
        <div class="fx2">

            <a href="#">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.unsplash.com/photo-1461611034385-e082102d5c75?auto=format&fit=crop&w=1050&q=60&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D">
                    <h4>title image</h4>
                    <p>Description</p>
                </div>
            </a>
            <a href="#">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.unsplash.com/photo-1461611034385-e082102d5c75?auto=format&fit=crop&w=1050&q=60&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D">
                    <h4>title image</h4>
                    <p>Description</p>
                </div>
            </a>
            <a href="#">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.unsplash.com/photo-1461611034385-e082102d5c75?auto=format&fit=crop&w=1050&q=60&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D">
                    <h4>title image</h4>
                    <p>Description</p>
                </div>
            </a>
            
        </div> 
        
        
        <div class="fx3">

            <a href="#">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.unsplash.com/photo-1461611034385-e082102d5c75?auto=format&fit=crop&w=1050&q=60&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D">
                    <h4>title image</h4>
                    <p>Description</p>
                </div>
            </a>
            <a href="#">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.unsplash.com/photo-1461611034385-e082102d5c75?auto=format&fit=crop&w=1050&q=60&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D">
                    <h4>title image</h4>
                    <p>Description</p>
                </div>
            </a>
            <a href="#">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.unsplash.com/photo-1461611034385-e082102d5c75?auto=format&fit=crop&w=1050&q=60&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D">
                    <h4>title image</h4>
                    <p>Description</p>
                </div>
            </a>
            
        </div> 
        
        
        <div class="fx5">

            <a href="#">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.unsplash.com/photo-1461611034385-e082102d5c75?auto=format&fit=crop&w=1050&q=60&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D">
                    <h4>title image</h4>
                    <p>Description</p>
                </div>
            </a>
            <a href="#">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.unsplash.com/photo-1461611034385-e082102d5c75?auto=format&fit=crop&w=1050&q=60&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D">
                    <h4>title image</h4>
                    <p>Description</p>
                </div>
            </a>
            <a href="#">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.unsplash.com/photo-1461611034385-e082102d5c75?auto=format&fit=crop&w=1050&q=60&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D">
                    <h4>title image</h4>
                    <p>Description</p>
                </div>
            </a>
            
        </div> 
         

    </div>
</div>



<iframe src="https://player.vimeo.com/video/997865296?h=715e669524&color=7a1818&title=0&byline=0&portrait=0" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>

Gallery video of Ann Marie Stillion's "Anonymous Sorrow" <br>

https://www.arttrek.com/ <br>
https://www.coregallery.org/ann-marie-stillion <b>

Director: Ann Marie Stillion @annmariestillion <br>
Editor: Deana Seitz @joybirdstudios <br>
Cinematography & Color Grade: Aster Teter @joybirdstudios <br>
Camera Assistant: Drew Boysen @drew.boysen <br>


<img src="{{site.baseurl}}/assets/img/as-2.jpg">