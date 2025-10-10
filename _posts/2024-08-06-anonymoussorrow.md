---
layout: post
title: "Anonymous Sorrow - Ann Marie Stillion"
author: "Deana Seitz and Aster Teter"
categories: gallery
tags: [gallery, color grading, editing]
image: as-1.jpg
---


<div class="browser" url="https://www.example.org/">
    <div class="iframe-wrapper">
      <iframe src="https://www.example.org/" frameborder="0">      
      </iframe>
    </div>
</div>

<style>
html,body {
  margin: 0;
  padding: 0;
}
// credit to nikkk-me for the browser mockup
* {
  box-sizing: border-box;
}

$red: #EB7061;
$yellow: #F5D160;
$green: #81D982;
$grey: #efefef;
$white: #ffffff;
$black: #333333;

$bigDotSize: 6px;
$smallDotSize: 2px;

//background
body {
  -webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
  font-family: sans-serif;
  background: white;
  color: $black;
  font-weight: 300;
  font-size: 14px;
}

.browser {
  position: relative;
  background: white;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15), 0 6px 10px rgba(0, 0, 0, 0.1);
  min-height: 500px;
  max-width: 80%;
  margin: auto;
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
  padding-top: 45px;
  background-image: radial-gradient(circle, $red $bigDotSize, transparent $bigDotSize),radial-gradient(circle, $yellow $bigDotSize, transparent $bigDotSize),radial-gradient(circle, $green $bigDotSize, transparent $bigDotSize), radial-gradient(circle, darken($grey, 12%) $smallDotSize, transparent $smallDotSize),radial-gradient(circle, darken($grey, 12%) $smallDotSize, transparent $smallDotSize),radial-gradient(circle, darken($grey, 12%) $smallDotSize, transparent $smallDotSize), linear-gradient(to bottom, $grey 45px, transparent 0);
  background-position:  left top, left top, left top, right top, right top, right top, 0 0;
  background-size:  50px 45px, 90px 45px, 130px 45px, 50px 30px, 50px 45px, 50px 60px, 100%;
  background-repeat: no-repeat, no-repeat;

  &[url]:after {
    content: attr(url);
    color: darken($grey, 30%);
    font-size: 13px;
    font-weight: 400;
    position: absolute;
    left: 0;
    right: 0;
    top: 0;
    padding: 6px 15px;
    margin: 9px 50px 0 90px;
    border-radius: 25px;
    background: $white;
    height: 27px;
    box-sizing: border-box;
  }
}

.iframe-wrapper {
  position: relative;
  overflow: hidden;
  padding-top: 56.25%;
  
  iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border: 0;
  }
}
</style>


<br>
original
<iframe src="https://player.vimeo.com/video/997865296?h=715e669524&color=7a1818&title=0&byline=0&portrait=0" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>

Gallery video of Ann Marie Stillion's "Anonymous Sorrow" <br>

https://www.arttrek.com/ <br>
https://www.coregallery.org/ann-marie-stillion <b>

Director: Ann Marie Stillion @annmariestillion <br>
Editor: Deana Seitz @joybirdstudios <br>
Cinematography & Color Grade: Aster Teter @joybirdstudios <br>
Camera Assistant: Drew Boysen @drew.boysen <br>


<img src="{{site.baseurl}}/assets/img/as-2.jpg">
<br>
new
<br>
<style>
@import url("https://fonts.googleapis.com/css?family=Raleway|Rozha+One");
</style>

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        /* Gallery Styles */
        .photo-gallery {
            max-width: 100%;
            margin: 20px auto;
            font-family: Raleway, sans-serif;
        }
        
        .gallery-title {
            text-align: center;
            margin-bottom: 20px;
            color: white;
            font-size: 24px;
        }
        
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 15px;
            padding: 10px;
        }
        
        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 0px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            aspect-ratio: 1 / 1;
        }
        
        .gallery-item:hover {
  opacity: 0.9;
  transform: scale(0.95);
        }
        
        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
            transition: transform 0.5s ease;
        }
        
        .image-caption {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            color: white;
            letter-spacing: 2px;
            position: absolute;
            top: 50%;
            left: 0;
            right: 0;
            margin: 0 auto;
            text-align: center;
            transition: all 0.3s ease;
            font-size: 14px;
            text-align: center;
            filter: blur(3px); /* make 3 */
            opacity: 0; /* make 0 */
        }
        
        .gallery-item:hover .image-caption {
            transform: translateY(0);
            filter: blur(0px);
  opacity: 1;
        }
        
        /* Responsive adjustments */
        @media (max-width: 768px) {
            .gallery-grid {
                grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
                gap: 10px;
            }
        }
        
        @media (max-width: 480px) {
            .gallery-grid {
                grid-template-columns: repeat(auto-fill, minmax(120px, 1fr));
                gap: 8px;
            }
            
            .gallery-title {
                font-size: 20px;
            }
        }
    </style>
</head>
<body>
    <div class="photo-gallery">
        <div class="gallery-grid">
            <!-- Gallery Item 1 -->
            <div class="gallery-item">
                <img src="https://images.unsplash.com/photo-1501854140801-50d01698950b?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Mountain landscape">
                <div class="image-caption">Mountain Landscape</div>
            </div>
            
            <!-- Gallery Item 2 -->
            <div class="gallery-item">
                <img src="https://images.unsplash.com/photo-1470071459604-3b5ec3a7fe05?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Forest path">
                <div class="image-caption">Forest Path</div>
            </div> 
            
            <!-- Gallery Item 3 -->
            <div class="gallery-item">
                <img src="https://images.unsplash.com/photo-1439066615861-d1af74d74000?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Lake view">
                <div class="image-caption">Lake View</div>
            </div>
            
            <!-- Gallery Item 4 -->
            <div class="gallery-item">
                <img src="https://images.unsplash.com/photo-1465146344425-f00d5f5c8f07?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Beach sunset">
                <div class="image-caption">Beach Sunset</div>
            </div>
            
            <!-- Gallery Item 5 -->
            <div class="gallery-item">
                <img src="https://images.unsplash.com/photo-1506905925346-21bda4d32df4?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Mountain peaks">
                <div class="image-caption">Mountain Peaks</div>
            </div>
            
            <!-- Gallery Item 6 -->
            <div class="gallery-item">
                <img src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Misty forest">
                <div class="image-caption">Misty Forest</div>
            </div>
        </div>
    </div>
</body>
</html>
