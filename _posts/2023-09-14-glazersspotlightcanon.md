---
layout: post
title: "Glazer's Camera Spotlight with Canon"
author: "Deana Seitz and Aster Teter"
categories: documentary
tags: [lifestyle, advertisement, documentary, editing, color grading, test 2 2023-04-23,]
image: canon2.jpg
---

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/Oi2GmQjwhX4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

Lead Editor: Deana Seitz

<br>

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Image Gallery</title>
    <style>
        /* Import fonts */
        @import url("https://fonts.googleapis.com/css?family=Raleway|Rozha+One");
        
        /* Scoped gallery styles to prevent conflicts */
        .gallery-container {
            --gallery-primary-color: #fff;
            --gallery-secondary-color: rgba(0, 0, 0, 0.9);
            --gallery-transition-duration: 0.5s;
            margin-bottom: 40px; /* Added space to prevent footer wrapping */
        }
        
        .gallery-container .col4 {
            width: 25%; /* Changed from 33.33% to 25% for 4 images */
            float: left;
            position: relative;
        }

        .gallery-container .transition {
            transition: all var(--gallery-transition-duration) ease;
        }

        .gallery-container .container {
            width: 90%; /* Increased from 70% to 90% for larger container */
            margin: 0 auto;
            overflow: hidden; /* Clear float */
        }

        .gallery-container .fx2 .item {
            margin: 10px;
            padding: 0;
            cursor: pointer;
            overflow: hidden;
        }

        .gallery-container .fx2 .item img {
            padding: 0 !important;
            display: block;
            max-width: 100%;
            height: auto;
            width: 100%;
        }

        .gallery-container .fx2 .image-link:hover .item img,
        .gallery-container .fx2 .image-link:focus .item img {
            opacity: 0.9;
            transform: scale(0.95);
        }

        .gallery-container .fx2 h4,
        .gallery-container .fx2 p {
            transition: all var(--gallery-transition-duration) ease;
        }

        .gallery-container .fx2 .image-link .item h4 {
            font-family: "Raleway", sans-serif;
            font-size: 16px;
            color: var(--gallery-primary-color);
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
            pointer-events: none;
        }

        .gallery-container .fx2 .image-link:hover .item h4,
        .gallery-container .fx2 .image-link:focus .item h4 {
            filter: blur(0px);
            opacity: 1;
        }

        .gallery-container .fx2 .image-link .item p {
            font-family: "Raleway", sans-serif;
            font-size: 8px;
            color: var(--gallery-primary-color);
            text-transform: uppercase;
            letter-spacing: 2px;
            position: absolute;
            top: 53%;
            left: 0;
            right: 0;
            margin: 0 auto;
            text-align: center;
            opacity: 0;
            pointer-events: none;
        }

        .gallery-container .fx2 .image-link:hover .item p,
        .gallery-container .fx2 .image-link:focus .item p {
            opacity: 1;
        }

        /* Modal Styles - Using :target selector */
        .gallery-container .modal {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--gallery-secondary-color);
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
            z-index: 1000;
            pointer-events: none;
            padding: 20px;
            box-sizing: border-box;
        }

        .gallery-container .modal:target {
            opacity: 1;
            visibility: visible;
            pointer-events: auto;
        }

        .gallery-container .modal-close {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            cursor: pointer;
            z-index: 1;
        }

        .gallery-container .modal-content {
            position: relative;
            max-width: 90%;
            max-height: 90%;
            text-align: center;
            transform: scale(0.8);
            transition: transform 0.3s ease;
            z-index: 2;
        }

        .gallery-container .modal:target .modal-content {
            transform: scale(1);
        }

        .gallery-container .modal-image {
            max-width: 100%;
            max-height: 80vh;
            height: auto;
            display: block;
            margin: 0 auto;
        }

        /* Animated Close Button - Improved positioning */
        .gallery-container .close-button {
            height: 50px;
            width: 50px;
            position: fixed; /* Changed from absolute to fixed for better mobile positioning */
            top: -60px;
            right: -60px;
            box-sizing: border-box;
            line-height: 50px;
            display: inline-block;
            cursor: pointer;
            background: rgba(0, 0, 0, 0.7);
            border-radius: 50%;
            transition: background 0.3s ease;
            z-index: 3;
        }

        .gallery-container .close-button:before, 
        .gallery-container .close-button:after {
            transform: rotate(-45deg);
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            margin-top: -2px;
            margin-left: -15px;
            display: block;
            height: 4px;
            width: 30px;
            background-color: #fff;
            transition: all 0.2s ease-out;
            border-radius: 2px;
        }

        .gallery-container .close-button:after {
            transform: rotate(45deg);
        }

        .gallery-container .close-button:hover {
            background: rgba(0, 0, 0, 0.9);
        }

        .gallery-container .close-button:hover:before, 
        .gallery-container .close-button:hover:after {
            transform: rotate(0deg);
        }

        /* Hide the fallback element */
        .gallery-container #close {
            display: none;
        }

        @media screen and (max-width: 991px) {
            .gallery-container .col4 {
                width: 50%;
            }
            .gallery-container .close-button {
                right: 0;
                top: -70px;
            }
            
            /* Prevent zoom on mobile */
            .gallery-container .modal {
                touch-action: manipulation;
            }
            
            .gallery-container .modal-content {
                max-width: 95%;
            }
        }

        @media screen and (max-width: 580px) {
            .gallery-container .col4 {
                width: 100%;
            }
            .gallery-container .modal-content {
                max-width: 98%;
            }
            .gallery-container .close-button {
                right: 0px;
                top: -60px;
                height: 40px;
                width: 40px;
            }
            
            .gallery-container .close-button:before, 
            .gallery-container .close-button:after {
                margin-top: -1.5px;
                margin-left: -12px;
                height: 3px;
                width: 24px;
            }
            
            /* Ensure content fits on mobile */
            .gallery-container .modal-image {
                max-height: 70vh;
            }
        }
    </style>
</head>
<body>
    <!-- Gallery Container -->
    <div class="gallery-container">
        <div class="container">
            <div class="fx2">
                <!-- Image 1 -->
                <a href="#image1" class="image-link">
                    <div class="item col4">
                        <img class="transition img-responsive" src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg">
                        <h4>Mountain View</h4>
                        <p>Beautiful mountain landscape</p>
                    </div>
                </a>
                
                <!-- Image 2 -->
                <a href="#image2" class="image-link">
                    <div class="item col4">
                        <img class="transition img-responsive" src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg">
                        <h4>Forest Path</h4>
                        <p>Serene forest trail</p>
                    </div>
                </a>
                
                <!-- Image 3 -->
                <a href="#image3" class="image-link">
                    <div class="item col4">
                        <img class="transition img-responsive" src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg">
                        <h4>Ocean Sunset</h4>
                        <p>Stunning ocean view</p>
                    </div>
                </a>
                
                <!-- Image 4 -->
                <a href="#image4" class="image-link">
                    <div class="item col4">
                        <img class="transition img-responsive" src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg">
                        <h4>City Lights</h4>
                        <p>Urban nightscape</p>
                    </div>
                  <!-- Image 4 -->
                <a href="#image4" class="image-link">
                    <div class="item col4">
                        <img class="transition img-responsive" src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg">
                        <h4>City Lights</h4>
                        <p>Urban nightscape</p>
                    </div>
                  <!-- Image 4 -->
                <a href="#image4" class="image-link">
                    <div class="item col4">
                        <img class="transition img-responsive" src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg">
                        <h4>City Lights</h4>
                        <p>Urban nightscape</p>
                    </div>
                </a>
            </div> 
        </div>

        <!-- Modals -->
        <div class="modal" id="image1">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg" class="modal-image">
                <a href="#" class="close-button"></a>
            </div>
        </div>

        <div class="modal" id="image2">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg" class="modal-image">
                <a href="#" class="close-button"></a>
            </div>
        </div>

        <div class="modal" id="image3">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg" class="modal-image">
                <a href="#" class="close-button"></a>
            </div>
        </div>
        
        <div class="modal" id="image4">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg" class="modal-image">
                <a href="#" class="close-button"></a>
            </div>
        </div>

        <!-- Fallback for closing -->
        <div id="close"></div>
    </div>
    
</body>
</html>
