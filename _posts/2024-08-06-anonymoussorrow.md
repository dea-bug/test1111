---
layout: post
title: "Anonymous Sorrow - Ann Marie Stillion"
author: "Deana Seitz and Aster Teter"
categories: gallery
tags: [gallery, color grading, editing]
image: as-1.jpg
---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Photo Gallery Widget</title>
    <style>
        /* Gallery Styles */
        .photo-gallery {
            max-width: 100%;
            margin: 20px auto;
            font-family: Arial, sans-serif;
        }
        
        .gallery-title {
            text-align: center;
            margin-bottom: 20px;
            color: #333;
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
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            aspect-ratio: 1 / 1;
        }
        
        .gallery-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 16px rgba(0,0,0,0.2);
        }
        
        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
            transition: transform 0.5s ease;
        }
        
        .gallery-item:hover img {
            transform: scale(1.05);
        }
        
        .image-caption {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: rgba(0,0,0,0.7);
            color: white;
            padding: 10px;
            transform: translateY(100%);
            transition: transform 0.3s ease;
            font-size: 14px;
            text-align: center;
        }
        
        .gallery-item:hover .image-caption {
            transform: translateY(0);
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
        <h2 class="gallery-title">My Photo Gallery</h2>
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