---
layout: post
title: "Anonymous Sorrow - Ann Marie Stillion"
author: "Deana Seitz and Aster Teter"
categories: gallery
tags: [gallery, color grading, editing]
image: as-1.jpg
---

<style>
@import url("https://fonts.googleapis.com/css?family=Raleway|Rozha+One");

.col4 {
  width: 33.33333333%;
  float: left;
  position: relative;
}

.transition {
  transition: all 0.5s ease;
}

.container {
  width: 33.333%;
  margin: 1 auto;
}

.fx2 .item {
  margin: 10px 0;
  padding: 0;
  cursor: pointer;
}

.fx2 .item img {
  padding: 0 !important;
  display: block;
  max-width: 100%;
  height: auto;
}

.fx2 .image-link:hover .item img,
.fx2 .image-link:focus .item img {
  opacity: 0.9;
  transform: scale(0.95);
}

.fx2 h4,
.fx2 p {
  transition: all 0.5s ease;
}

.fx2 .image-link .item h4 {
  font-family: "Raleway", sans-serif;
  font-size: 16px;
  color: #fff;
  text-transform: uppercase;
  letter-spacing: 2px;
  position: absolute;
  top: 42%;
  left: 0;
  right: 0;
  margin: 0 auto;
  text-align: center;
  filter: blur(5px);
  opacity: 0;
}

.fx2 .image-link:hover .item h4,
.fx2 .image-link:focus .item h4 {
  filter: blur(0px);
  opacity: 1;
}

.fx2 .image-link .item p {
  font-family: "Raleway", sans-serif;
  font-size: 8px;
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

.fx2 .image-link:hover .item p,
.fx2 .image-link:focus .item p {
  opacity: 1;
}

/* Modal Styles - Using :target selector */
.modal {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.9);
  display: flex;
  align-items: center;
  justify-content: center;
  opacity: 0;
  visibility: hidden;
  transition: all 0.3s ease;
  z-index: 1000;
  pointer-events: none;
}

.modal:target {
  opacity: 1;
  visibility: visible;
  pointer-events: auto;
}

.modal-close {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  cursor: pointer;
  z-index: 1;
}

.modal-content {
  position: relative;
  max-width: 90%;
  max-height: 90%;
  text-align: center;
  transform: scale(0.8);
  transition: transform 0.3s ease;
  z-index: 2;
}

.modal:target .modal-content {
  transform: scale(1);
}

.modal-image {
  max-width: 100%;
  max-height: 80vh;
  height: auto;
  display: block;
}

.close-btn {
  position: absolute;
  top: -50px;
  right: -50px;
  color: white;
  font-size: 40px;
  cursor: pointer;
  background: rgba(0, 0, 0, 0.7);
  width: 50px;
  height: 50px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  transition: background 0.3s ease;
  z-index: 3;
}

.close-btn:hover {
  background: rgba(0, 0, 0, 0.9);
}

/* Hide the fallback element */
#close {
  display: none;
}

@media screen and (max-width: 991px) {
  .col4 {
    width: 50%;
  }
  .close-btn {
    right: 0;
    top: -60px;
  }
}

@media screen and (max-width: 580px) {
  .col4 {
    width: 100%;
  }
  .modal-content {
    max-width: 95%;
  }
  .close-btn {
    right: 0;
    top: -50px;
    font-size: 30px;
    width: 40px;
    height: 40px;
  }
}

</style>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vimeo Gallery</title>
    <style>
        /* Reset and base styles */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            line-height: 1.6;
            color: #333;
            /* Removed background color */
            padding: 0; /* Fixed padding issue causing right shift */
        }

        /* Gallery container */
        .gallery-container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto 30px;
            overflow: hidden;
        }

        .fx2 {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            margin: 0 -10px;
        }

        .col4 {
            width: 33.33333333%;
            padding: 10px;
            position: relative;
        }

        .transition {
            transition: all 0.5s ease;
        }

        .fx2 .item {
            margin: 0;
            padding: 0;
            cursor: pointer;
            overflow: hidden;
        }

        .fx2 .item img {
            padding: 0 !important;
            display: block;
            width: 100%;
            height: auto;
        }

        .fx2 .image-link:hover .item img,
        .fx2 .image-link:focus .item img {
            opacity: 0.9;
            transform: scale(0.95);
        }

        .fx2 h4,
        .fx2 p {
            transition: all 0.5s ease;
        }

        .fx2 .image-link .item h4 {
            font-family: "Raleway", sans-serif;
            font-size: 16px;
            color: #fff;
            text-transform: uppercase;
            letter-spacing: 2px;
            position: absolute;
            top: 42%;
            left: 0;
            right: 0;
            margin: 0 auto;
            text-align: center;
            filter: blur(5px);
            opacity: 0;
        }

        .fx2 .image-link:hover .item h4,
        .fx2 .image-link:focus .item h4 {
            filter: blur(0px);
            opacity: 1;
        }

        .fx2 .image-link .item p {
            font-family: "Raleway", sans-serif;
            font-size: 8px;
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

        .fx2 .image-link:hover .item p,
        .fx2 .image-link:focus .item p {
            opacity: 1;
        }

        /* Video container - matches gallery width */
        .video-container {
            width: 100%;
            max-width: 640px;
            margin: 0 auto;
            padding: 10px;
        }

        .video-wrapper {
            position: relative;
            padding-bottom: 56.25%; /* 16:9 aspect ratio */
            height: 0;
            overflow: hidden;
        }

        .video-wrapper iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: none;
        }

        /* Modal Styles */
        .modal {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.9);
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
            z-index: 1000;
            pointer-events: none;
        }

        .modal:target {
            opacity: 1;
            visibility: visible;
            pointer-events: auto;
        }

        .modal-close {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            cursor: pointer;
            z-index: 1;
        }

        .modal-content {
            position: relative;
            max-width: 90%;
            max-height: 90%;
            text-align: center;
            transform: scale(0.8);
            transition: transform 0.3s ease;
            z-index: 2;
        }

        .modal:target .modal-content {
            transform: scale(1);
        }

        .modal-image {
            max-width: 100%;
            max-height: 80vh;
            height: auto;
            display: block;
        }

        .close-btn {
            position: absolute;
            top: -50px;
            right: -50px;
            color: white;
            font-size: 40px;
            cursor: pointer;
            background: rgba(0, 0, 0, 0.7);
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            text-decoration: none;
            transition: background 0.3s ease;
            z-index: 3;
        }

        .close-btn:hover {
            background: rgba(0, 0, 0, 0.9);
        }

        /* Hide the fallback element */
        #close {
            display: none;
        }

        /* Responsive adjustments */
        @media screen and (max-width: 991px) {
            .col4 {
                width: 50%;
            }
            .close-btn {
                right: 0;
                top: -60px;
            }
        }

        @media screen and (max-width: 768px) {
            .video-container {
                padding: 5px;
            }
        }

        @media screen and (max-width: 580px) {
            .col4 {
                width: 100%;
            }
            .modal-content {
                max-width: 95%;
            }
            .close-btn {
                right: 0;
                top: -50px;
                font-size: 30px;
                width: 40px;
                height: 40px;
            }
        }
    </style>
</head>
<body>
    <!-- Image Gallery -->
    <div class="gallery-container">
        <div class="fx2">
            <!-- Image 1 -->
            <a href="#image1" class="image-link">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.unsplash.com/photo-1461611034385-e082102d5c75?auto=format&fit=crop&w=1050&q=60&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D">
                    <h4>Title Image 1</h4>
                    <p>Description for image 1</p>
                </div>
            </a>
            
            <!-- Image 2 -->
            <a href="#image2" class="image-link">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.unsplash.com/photo-1506905925346-21bda4d32df4?auto=format&fit=crop&w=1050&q=60">
                    <h4>Title Image 2</h4>
                    <p>Description for image 2</p>
                </div>
            </a>
            
            <!-- Image 3 -->
            <a href="#image3" class="image-link">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.unsplash.com/photo-1501785888041-af3ef285b470?auto=format&fit=crop&w=1050&q=60">
                    <h4>Title Image 3</h4>
                    <p>Description for image 3</p>
                </div>
            </a>
        </div> 
    </div>

    <!-- Vimeo Video -->
    <div class="video-container">
        <div class="video-wrapper">
            <iframe src="https://player.vimeo.com/video/997865296?h=715e669524&color=7a1818&title=0&byline=0&portrait=0" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
        </div>
    </div>

    <!-- Modals -->
    <div class="modal" id="image1">
        <a href="#" class="modal-close"></a>
        <div class="modal-content">
            <img src="https://images.unsplash.com/photo-1461611034385-e082102d5c75?auto=format&fit=crop&w=1050&q=60&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D" class="modal-image">
            <a href="#" class="close-btn">&times;</a>
        </div>
    </div>

    <div class="modal" id="image2">
        <a href="#" class="modal-close"></a>
        <div class="modal-content">
            <img src="https://images.unsplash.com/photo-1506905925346-21bda4d32df4?auto=format&fit=crop&w=1050&q=60" class="modal-image">
            <a href="#" class="close-btn">&times;</a>
        </div>
    </div>

    <div class="modal" id="image3">
        <a href="#" class="modal-close"></a>
        <div class="modal-content">
            <img src="https://images.unsplash.com/photo-1501785888041-af3ef285b470?auto=format&fit=crop&w=1050&q=60" class="modal-image">
            <a href="#" class="close-btn">&times;</a>
        </div>
    </div>

    <!-- Fallback for closing -->
    <div id="close"></div>
</body>
</html>

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