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

New Versions

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Four Photo Gallery Designs</title>
    <link href="https://fonts.googleapis.com/css2?family=Raleway:wght@400;500;600&family=Rozha+One&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Raleway', sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f9f9f9;
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        header {
            text-align: center;
            margin-bottom: 40px;
            padding: 20px;
        }
        
        h1 {
            font-family: 'Rozha One', serif;
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: #2c3e50;
        }
        
        .subtitle {
            font-size: 1.2rem;
            color: #7f8c8d;
            max-width: 700px;
            margin: 0 auto;
        }
        
        .gallery-container {
            margin-bottom: 60px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            overflow: hidden;
        }
        
        .gallery-title {
            font-family: 'Rozha One', serif;
            font-size: 1.8rem;
            padding: 20px;
            background: #2c3e50;
            color: white;
            text-align: center;
        }
        
        .gallery-description {
            padding: 15px 20px;
            background: #f1f2f6;
            color: #555;
            font-style: italic;
            text-align: center;
        }
        
        /* Gallery 1: Classic Grid */
        .classic-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 15px;
            padding: 20px;
        }
        
        .classic-item {
            position: relative;
            overflow: hidden;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            aspect-ratio: 1 / 1;
        }
        
        .classic-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 16px rgba(0,0,0,0.2);
        }
        
        .classic-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
            transition: transform 0.5s ease;
        }
        
        .classic-item:hover img {
            transform: scale(1.05);
        }
        
        .classic-caption {
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
        
        .classic-item:hover .classic-caption {
            transform: translateY(0);
        }
        
        /* Gallery 2: Masonry Style */
        .masonry-grid {
            columns: 4 250px;
            column-gap: 15px;
            padding: 20px;
        }
        
        .masonry-item {
            break-inside: avoid;
            margin-bottom: 15px;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
            background: white;
        }
        
        .masonry-item:hover {
            transform: scale(1.02);
        }
        
        .masonry-item img {
            width: 100%;
            display: block;
        }
        
        .masonry-caption {
            padding: 10px;
            text-align: center;
            background: white;
            font-size: 14px;
            color: #555;
        }
        
        /* Gallery 3: Card Style */
        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 25px;
            padding: 20px;
        }
        
        .card-item {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .card-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.15);
        }
        
        .card-image {
            height: 200px;
            overflow: hidden;
        }
        
        .card-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .card-item:hover .card-image img {
            transform: scale(1.1);
        }
        
        .card-content {
            padding: 20px;
        }
        
        .card-content h3 {
            font-size: 1.2rem;
            margin-bottom: 10px;
            color: #2c3e50;
        }
        
        .card-content p {
            color: #7f8c8d;
            font-size: 0.9rem;
        }
        
        /* Gallery 4: Modal Gallery (inspired by provided code) */
        .modal-gallery {
            padding: 20px;
        }
        
        .fx2 {
            display: flex;
            flex-wrap: wrap;
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
        
        .item {
            margin: 10px 0;
            padding: 0;
            cursor: pointer;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        
        .item img {
            padding: 0 !important;
            display: block;
            max-width: 100%;
            height: auto;
        }
        
        .image-link:hover .item img,
        .image-link:focus .item img {
            opacity: 0.9;
            transform: scale(0.95);
        }
        
        .fx2 h4,
        .fx2 p {
            transition: all 0.5s ease;
        }
        
        .image-link .item h4 {
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
        
        .image-link:hover .item h4,
        .image-link:focus .item h4 {
            filter: blur(0px);
            opacity: 1;
        }
        
        .image-link .item p {
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
        
        .image-link:hover .item p,
        .image-link:focus .item p {
            opacity: 1;
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
            border-radius: 5px;
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
            .classic-grid {
                grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            }
            
            .masonry-grid {
                columns: 2 200px;
            }
            
            .card-grid {
                grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
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
            
            .classic-grid,
            .masonry-grid,
            .card-grid {
                grid-template-columns: 1fr;
                columns: 1;
            }
        }
        
        footer {
            text-align: center;
            margin-top: 40px;
            padding: 20px;
            color: #7f8c8d;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>
    <header>
        <h1>Four Photo Gallery Designs</h1>
        <p class="subtitle">Choose from these four distinct gallery styles to showcase your photos in any blog post or website</p>
    </header>
    
    <!-- Gallery 1: Classic Grid -->
    <div class="gallery-container">
        <h2 class="gallery-title">Classic Grid Gallery</h2>
        <p class="gallery-description">A clean, responsive grid with hover effects and captions</p>
        <div class="classic-grid">
            <div class="classic-item">
                <img src="https://images.unsplash.com/photo-1501854140801-50d01698950b?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Mountain landscape">
                <div class="classic-caption">Mountain Landscape</div>
            </div>
            <div class="classic-item">
                <img src="https://images.unsplash.com/photo-1470071459604-3b5ec3a7fe05?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Forest path">
                <div class="classic-caption">Forest Path</div>
            </div>
            <div class="classic-item">
                <img src="https://images.unsplash.com/photo-1439066615861-d1af74d74000?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Lake view">
                <div class="classic-caption">Lake View</div>
            </div>
            <div class="classic-item">
                <img src="https://images.unsplash.com/photo-1465146344425-f00d5f5c8f07?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Beach sunset">
                <div class="classic-caption">Beach Sunset</div>
            </div>
            <div class="classic-item">
                <img src="https://images.unsplash.com/photo-1506905925346-21bda4d32df4?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Mountain peaks">
                <div class="classic-caption">Mountain Peaks</div>
            </div>
            <div class="classic-item">
                <img src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Misty forest">
                <div class="classic-caption">Misty Forest</div>
            </div>
        </div>
    </div>
    
    <!-- Gallery 2: Masonry Style -->
    <div class="gallery-container">
        <h2 class="gallery-title">Masonry Style Gallery</h2>
        <p class="gallery-description">A Pinterest-style layout with varying image heights</p>
        <div class="masonry-grid">
            <div class="masonry-item">
                <img src="https://images.unsplash.com/photo-1501854140801-50d01698950b?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Mountain landscape">
                <div class="masonry-caption">Mountain Landscape</div>
            </div>
            <div class="masonry-item">
                <img src="https://images.unsplash.com/photo-1470071459604-3b5ec3a7fe05?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Forest path">
                <div class="masonry-caption">Forest Path</div>
            </div>
            <div class="masonry-item">
                <img src="https://images.unsplash.com/photo-1439066615861-d1af74d74000?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Lake view">
                <div class="masonry-caption">Lake View</div>
            </div>
            <div class="masonry-item">
                <img src="https://images.unsplash.com/photo-1465146344425-f00d5f5c8f07?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Beach sunset">
                <div class="masonry-caption">Beach Sunset</div>
            </div>
            <div class="masonry-item">
                <img src="https://images.unsplash.com/photo-1506905925346-21bda4d32df4?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Mountain peaks">
                <div class="masonry-caption">Mountain Peaks</div>
            </div>
            <div class="masonry-item">
                <img src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Misty forest">
                <div class="masonry-caption">Misty Forest</div>
            </div>
        </div>
    </div>
    
    <!-- Gallery 3: Card Style -->
    <div class="gallery-container">
        <h2 class="gallery-title">Card Style Gallery</h2>
        <p class="gallery-description">Image cards with descriptive text and elegant hover effects</p>
        <div class="card-grid">
            <div class="card-item">
                <div class="card-image">
                    <img src="https://images.unsplash.com/photo-1501854140801-50d01698950b?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Mountain landscape">
                </div>
                <div class="card-content">
                    <h3>Mountain Landscape</h3>
                    <p>Breathtaking view of snow-capped mountains against a clear blue sky. Perfect for nature lovers and adventurers.</p>
                </div>
            </div>
            <div class="card-item">
                <div class="card-image">
                    <img src="https://images.unsplash.com/photo-1470071459604-3b5ec3a7fe05?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Forest path">
                </div>
                <div class="card-content">
                    <h3>Forest Path</h3>
                    <p>A serene path winding through a lush green forest. The play of light and shadow creates a magical atmosphere.</p>
                </div>
            </div>
            <div class="card-item">
                <div class="card-image">
                    <img src="https://images.unsplash.com/photo-1439066615861-d1af74d74000?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Lake view">
                </div>
                <div class="card-content">
                    <h3>Lake View</h3>
                    <p>Crystal clear lake surrounded by majestic mountains. The perfect spot for reflection and tranquility.</p>
                </div>
            </div>
            <div class="card-item">
                <div class="card-image">
                    <img src="https://images.unsplash.com/photo-1465146344425-f00d5f5c8f07?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Beach sunset">
                </div>
                <div class="card-content">
                    <h3>Beach Sunset</h3>
                    <p>Vibrant colors paint the sky as the sun sets over the ocean. A moment of pure peace and beauty.</p>
                </div>
            </div>
        </div>
    </div>
    
    <!-- Gallery 4: Modal Gallery -->
    <div class="gallery-container">
        <h2 class="gallery-title">Modal Gallery</h2>
        <p class="gallery-description">Click on images to view them in a full-screen modal with smooth transitions</p>
        <div class="modal-gallery">
            <div class="fx2">
                <!-- Image 1 -->
                <a href="#image1" class="image-link">
                    <div class="item col4">
                        <img class="transition img-responsive" src="https://images.unsplash.com/photo-1501854140801-50d01698950b?auto=format&fit=crop&w=1050&q=60">
                        <h4>Mountain Landscape</h4>
                        <p>Photo by Nature Lover</p>
                    </div>
                </a>
                
                <!-- Image 2 -->
                <a href="#image2" class="image-link">
                    <div class="item col4">
                        <img class="transition img-responsive" src="https://images.unsplash.com/photo-1470071459604-3b5ec3a7fe05?auto=format&fit=crop&w=1050&q=60">
                        <h4>Forest Path</h4>
                        <p>Photo by Forest Explorer</p>
                    </div>
                </a>
                
                <!-- Image 3 -->
                <a href="#image3" class="image-link">
                    <div class="item col4">
                        <img class="transition img-responsive" src="https://images.unsplash.com/photo-1439066615861-d1af74d74000?auto=format&fit=crop&w=1050&q=60">
                        <h4>Lake View</h4>
                        <p>Photo by Lake Photographer</p>
                    </div>
                </a>
                
                <!-- Image 4 -->
                <a href="#image4" class="image-link">
                    <div class="item col4">
                        <img class="transition img-responsive" src="https://images.unsplash.com/photo-1465146344425-f00d5f5c8f07?auto=format&fit=crop&w=1050&q=60">
                        <h4>Beach Sunset</h4>
                        <p>Photo by Sunset Chaser</p>
                    </div>
                </a>
                
                <!-- Image 5 -->
                <a href="#image5" class="image-link">
                    <div class="item col4">
                        <img class="transition img-responsive" src="https://images.unsplash.com/photo-1506905925346-21bda4d32df4?auto=format&fit=crop&w=1050&q=60">
                        <h4>Mountain Peaks</h4>
                        <p>Photo by Mountain Adventurer</p>
                    </div>
                </a>
                
                <!-- Image 6 -->
                <a href="#image6" class="image-link">
                    <div class="item col4">
                        <img class="transition img-responsive" src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e?auto=format&fit=crop&w=1050&q=60">
                        <h4>Misty Forest</h4>
                        <p>Photo by Mist Hunter</p>
                    </div>
                </a>
            </div> 
        </div>
        
        <!-- Modals -->
        <div class="modal" id="image1">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://images.unsplash.com/photo-1501854140801-50d01698950b?auto=format&fit=crop&w=1050&q=60" class="modal-image">
                <a href="#" class="close-btn">&times;</a>
            </div>
        </div>

        <div class="modal" id="image2">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://images.unsplash.com/photo-1470071459604-3b5ec3a7fe05?auto=format&fit=crop&w=1050&q=60" class="modal-image">
                <a href="#" class="close-btn">&times;</a>
            </div>
        </div>

        <div class="modal" id="image3">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://images.unsplash.com/photo-1439066615861-d1af74d74000?auto=format&fit=crop&w=1050&q=60" class="modal-image">
                <a href="#" class="close-btn">&times;</a>
            </div>
        </div>
        
        <div class="modal" id="image4">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://images.unsplash.com/photo-1465146344425-f00d5f5c8f07?auto=format&fit=crop&w=1050&q=60" class="modal-image">
                <a href="#" class="close-btn">&times;</a>
            </div>
        </div>
        
        <div class="modal" id="image5">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://images.unsplash.com/photo-1506905925346-21bda4d32df4?auto=format&fit=crop&w=1050&q=60" class="modal-image">
                <a href="#" class="close-btn">&times;</a>
            </div>
        </div>
        
        <div class="modal" id="image6">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e?auto=format&fit=crop&w=1050&q=60" class="modal-image">
                <a href="#" class="close-btn">&times;</a>
            </div>
        </div>

        <!-- Fallback for closing -->
        <div id="close"></div>
    </div>
    
    <footer>
        <p>Four unique photo gallery designs - Perfect for embedding in blog posts and websites</p>
    </footer>
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