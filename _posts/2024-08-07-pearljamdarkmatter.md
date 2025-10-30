---
layout: post
author: "Deana Seitz and Aster Teter"
title: "Pearl Jam: Dark Matter World Tour 2024"
categories: music videos
tags: [music videos, color grading, editing, visuals]
image: pjdm-header.jpg
---
<!-- Header Animation -->
<div class="anim-header-container">
    <div class="anim-image-wrapper">
        <img src="https://snipboard.io/xh1kbv.jpg" alt="Animated concert ticket header image"> 
        <div class="anim-title-container">
            <span class="anim-title-line">------</span>
            <span class="anim-title-line">World Tour 2024</span>
        </div>
    </div>
</div>

<!-- Photo credit -->
<p style="font-size: 12px; color: grey; text-align: right; margin-top: 5px;">photos + BTS footage by ---</p>

<link href="https://fonts.googleapis.com/css2?family=Anton&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css?family=Raleway|Rozha+One|Montserrat:400,500,600,700&display=swap" rel="stylesheet">

<style>
/* Import Montserrat for all paragraph text */
.post-content p {
    font-family: 'Montserrat', sans-serif !important;
}

/* Force Montserrat on all regular paragraphs */
p:not([class*="anim-title-line"]):not([style*="color: grey"]) {
    font-family: 'Montserrat', sans-serif !important;
}

/* Header Animation Styles */
.anim-header-container {
    position: relative;
    width: 100%;
    max-width: 1500px;
    margin: 0 auto;
    overflow: hidden;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
    border-radius: 8px;
}

.anim-image-wrapper {
    position: relative;
    width: 100%;
    height: 0;
    padding-bottom: 33.33%;
    background-color: #222;
}

.anim-image-wrapper img {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.anim-title-container {
    position: absolute;
    bottom: 20px;
    left: 30px;
    width: 75%;
    max-width: 975px;
    font-family: 'Anton', sans-serif;
    color: white;
    text-transform: uppercase;
    overflow: hidden;
}

.anim-title-line {
    display: block;
    font-size: clamp(2rem, 2.5vw, 2.5rem);
    letter-spacing: -2px;
    line-height: 1;
    margin-bottom: 5px;
    opacity: 0;
    transform: translateY(80%);
    animation: anim-lineUp 3s ease-out forwards;
}

.anim-title-line:nth-child(1) {
    animation-delay: 0.2s;
}

.anim-title-line:nth-child(2) {
    animation-delay: 0.5s;
}

@keyframes anim-lineUp {
    0% {
        opacity: 0;
        transform: translateY(80%);
    }
    20% {
        opacity: 0;
    }
    50% {
        opacity: 1;
        transform: translateY(0%);
    }
    100% {
        opacity: 1;
        transform: translateY(0%);
    }
}

/* Gallery Styles - Fixed for horizontal stacking and larger modals */
.gallery-container {
    --gallery-primary-color: #fff;
    --gallery-secondary-color: rgba(0, 0, 0, 0.9);
    --gallery-transition-duration: 0.5s;
    margin-bottom: 40px;
    font-family: 'Montserrat', sans-serif;
    padding: 20px;
    background: #fff;
}

.gallery-container .col4 {
    width: 33.333% !important; /* Force 3 columns for horizontal stacking */
    float: left;
    position: relative;
    box-sizing: border-box;
}

.gallery-container .transition {
    transition: all var(--gallery-transition-duration) ease;
}

.gallery-container .container {
    width: 100% !important; /* Full width for better horizontal layout */
    margin: 0 auto;
    overflow: hidden;
    display: block;
}

.gallery-container .fx2 {
    display: block;
    width: 100%;
    overflow: hidden;
}

.gallery-container .fx2 .item {
    margin: 10px;
    padding: 0;
    cursor: pointer;
    overflow: hidden;
    float: left; /* Ensure horizontal stacking */
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

/* Modal Styles - Made larger for readability */
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
    z-index: 10000; /* Higher z-index to overcome theme conflicts */
    pointer-events: none;
    padding: 10px; /* Reduced padding for larger modal */
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
    max-width: 95% !important; /* Larger modal for readability */
    max-height: 95% !important; /* Larger modal for readability */
    text-align: center;
    transform: scale(0.8);
    transition: transform 0.3s ease;
    z-index: 2;
}

.gallery-container .modal:target .modal-content {
    transform: scale(1);
}

.gallery-container .modal-image {
    max-width: 100% !important;
    max-height: 85vh !important; /* Larger image in modal */
    height: auto;
    display: block;
    margin: 0 auto;
}

.gallery-container .close-button {
    height: 50px;
    width: 50px;
    position: fixed;
    top: 20px !important; /* Better positioning */
    right: 20px !important; /* Better positioning */
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

.gallery-container #close {
    display: none;
}

/* Carousel Styles with higher specificity */
#isolated-carousel {
    all: initial !important;
    display: block !important;
    max-width: 900px;
    margin: 20px auto;
    padding: 20px;
    position: relative;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

#isolated-carousel .carousel-slides {
    all: initial !important;
    display: block !important;
    position: relative;
    height: 500px;
    overflow: hidden;
    border-radius: 8px;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
    box-sizing: border-box;
}

#isolated-carousel .carousel-slide {
    all: initial !important;
    display: block !important;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    opacity: 0;
    transition: opacity 0.5s ease-in-out;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #f5f5f5;
    box-sizing: border-box;
}

#isolated-carousel .carousel-slide.active {
    opacity: 1 !important;
}

#isolated-carousel .carousel-slide img {
    all: initial !important;
    display: block !important;
    max-width: 100%;
    max-height: 100%;
    width: auto;
    height: auto;
    object-fit: contain;
    box-sizing: border-box;
}

#isolated-carousel .carousel-arrow {
    all: initial !important;
    display: block !important;
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    background-color: rgba(0,0,0,0.5);
    color: white;
    border: none;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    font-size: 24px;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: background-color 0.3s;
    z-index: 10;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

#isolated-carousel .carousel-arrow:hover {
    background-color: grey;
}

#isolated-carousel .carousel-arrow.prev {
    left: 15px;
}

#isolated-carousel .carousel-arrow.next {
    right: 15px;
}

#isolated-carousel .carousel-dots {
    all: initial !important;
    display: flex !important;
    justify-content: center;
    margin-top: 20px;
    gap: 10px;
    box-sizing: border-box;
}

#isolated-carousel .carousel-dot {
    all: initial !important;
    display: block !important;
    width: 12px;
    height: 12px;
    border-radius: 50%;
    background-color: #ccc;
    cursor: pointer;
    transition: background-color 0.3s;
    box-sizing: border-box;
}

#isolated-carousel .carousel-dot.active {
    background-color: #333 !important;
}

/* Second Carousel Styles */
#isolated-carousel-2 {
    all: initial !important;
    display: block !important;
    max-width: 900px;
    margin: 20px auto;
    padding: 20px;
    position: relative;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

#isolated-carousel-2 .carousel-slides {
    all: initial !important;
    display: block !important;
    position: relative;
    height: 500px;
    overflow: hidden;
    border-radius: 80px;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
    box-sizing: border-box;
}

#isolated-carousel-2 .carousel-slide {
    all: initial !important;
    display: block !important;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    opacity: 0;
    transition: opacity 0.5s ease-in-out;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: black;
    box-sizing: border-box;
}

#isolated-carousel-2 .carousel-slide.active {
    opacity: 1 !important;
}

#isolated-carousel-2 .carousel-slide img {
    all: initial !important;
    display: block !important;
    max-width: 100%;
    max-height: 100%;
    width: auto;
    height: auto;
    object-fit: contain;
    box-sizing: border-box;
}

#isolated-carousel-2 .carousel-arrow {
    all: initial !important;
    display: block !important;
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    background-color: rgba(0,0,0,0.5);
    color: white;
    border: none;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    font-size: 24px;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: background-color 0.3s;
    z-index: 10;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

#isolated-carousel-2 .carousel-arrow:hover {
    background-color: rgba(0, 0, 0, 0.8);
}

#isolated-carousel-2 .carousel-arrow.prev {
    left: 15px;
}

#isolated-carousel-2 .carousel-arrow.next {
    right: 15px;
}

#isolated-carousel-2 .carousel-dots {
    all: initial !important;
    display: flex !important;
    justify-content: center;
    margin-top: 20px;
    gap: 10px;
    box-sizing: border-box;
}

#isolated-carousel-2 .carousel-dot {
    all: initial !important;
    display: block !important;
    width: 12px;
    height: 12px;
    border-radius: 50%;
    background-color: #ccc;
    cursor: pointer;
    transition: background-color 0.3s;
    box-sizing: border-box;
}

#isolated-carousel-2 .carousel-dot.active {
    background-color: #333 !important;
}

/* Mobile Responsiveness with horizontal gallery fix */
@media (max-width: 768px) {
    .anim-title-container {
        bottom: 15px;
        left: 15px;
    }
    
    .anim-title-line {
        margin-bottom: 3px;
    }
    
    .gallery-container .col4 {
        width: 50% !important; /* 2 columns on tablet */
    }
    
    .gallery-container .close-button {
        right: 10px !important;
        top: 10px !important;
    }
    
    .gallery-container .modal-content {
        max-width: 98% !important;
        max-height: 98% !important;
    }
    
    #isolated-carousel .carousel-slides,
    #isolated-carousel-2 .carousel-slides {
        height: 350px;
    }
    
    #isolated-carousel .carousel-arrow,
    #isolated-carousel-2 .carousel-arrow {
        width: 40px;
        height: 40px;
        font-size: 20px;
    }
}

@media (max-width: 480px) {
    .anim-title-container {
        bottom: 10px;
        left: 10px;
        width: 80%;
    }
    
    .gallery-container .col4 {
        width: 100% !important; /* 1 column on mobile but still horizontal flow */
        float: none;
        display: block;
        margin: 10px auto;
    }
    
    .gallery-container .container {
        overflow: visible;
    }
    
    .gallery-container .fx2 .item {
        float: none;
        display: block;
    }
    
    .gallery-container .modal-content {
        max-width: 99% !important;
        max-height: 99% !important;
    }
    
    .gallery-container .close-button {
        right: 5px !important;
        top: 5px !important;
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
    
    .gallery-container .modal-image {
        max-height: 75vh !important;
    }
    
    #isolated-carousel .carousel-slides,
    #isolated-carousel-2 .carousel-slides {
        height: 250px;
    }
    
    #isolated-carousel .carousel-arrow,
    #isolated-carousel-2 .carousel-arrow {
        width: 35px;
        height: 35px;
        font-size: 18px;
    }
    
    #isolated-carousel .carousel-dot,
    #isolated-carousel-2 .carousel-dot {
        width: 12px;
        height: 12px;
    }
}
</style>

<!-- Gallery Section -->
<div class="gallery-container">
    <div class="container">
        <div class="fx2">
            <!-- Image 1 -->
            <a href="#image1" class="image-link">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg" alt="Gallery image 1">
                </div>
            </a>
            
            <!-- Image 2 -->
            <a href="#image2" class="image-link">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg" alt="Gallery image 2">
                </div>
            </a>
            
            <!-- Image 3 -->
            <a href="#image3" class="image-link">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg" alt="Gallery image 3">
                </div>
            </a>
        </div>

        <!-- Gallery Modals -->
        <div class="modal" id="image1">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg" class="modal-image" alt="Modal image 1">
                <a href="#" class="close-button"></a>
            </div>
        </div>

        <div class="modal" id="image2">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg" class="modal-image" alt="Modal image 2">
                <a href="#" class="close-button"></a>
            </div>
        </div>

        <div class="modal" id="image3">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://images.pexels.com/photos/33915754/pexels-photo-33915754.jpeg" class="modal-image" alt="Modal image 3">
                <a href="#" class="close-button"></a>
            </div>
        </div>

        <div id="close"></div>
    </div>
</div>

<!-- Content Sections -->
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Vitae semper quis lectus nulla at volutpat diam</p>
<br>
<img src="https://snipboard.io/6R3jOh.jpg" alt="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Vitae semper quis lectus nulla at volutpat diam"> 
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Vitae semper quis lectus nulla at volutpat diam</p>

<!-- First Carousel - Fixed with placeholder images -->
<div id="isolated-carousel">
    <div class="carousel-slides">
        <!-- Slide 1 -->
        <div class="carousel-slide active">
            <img src="https://snipboard.io/6R3jOh.jpg" alt="Image 1">
        </div>
        
        <!-- Slide 2 -->
        <div class="carousel-slide">
            <img src="https://snipboard.io/6R3jOh.jpg" alt="Image 2">
        </div>
        
        <!-- Slide 3 -->
        <div class="carousel-slide">
            <img src="https://snipboard.io/6R3jOh.jpg" alt="Image 3">
        </div>
        
        <!-- Slide 4 -->
        <div class="carousel-slide">
            <img src="https://snipboard.io/6R3jOh.jpg" alt="Image 4">
        </div>
        
        <!-- Navigation Arrows -->
        <button class="carousel-arrow prev">&#10094;</button>
        <button class="carousel-arrow next">&#10095;</button>
    </div>
    
    <!-- Dots Indicator -->
    <div class="carousel-dots">
        <span class="carousel-dot active" data-index="0"></span>
        <span class="carousel-dot" data-index="1"></span>
        <span class="carousel-dot" data-index="2"></span>
        <span class="carousel-dot" data-index="3"></span>
    </div>
</div>

<br>

<!-- More Content -->
<center>
Take a glimpse of our process below:
<br>
[embedded and centered instagram content 1]
<br>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Vitae semper quis lectus nulla at volutpat diam</p>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Vitae semper quis lectus nulla at volutpat diam</p>
[embedded and centered instagram content 2]
<br>
</center>

<!-- Second Carousel - Fixed with placeholder images -->
<div id="isolated-carousel-2">
    <div class="carousel-slides">
        <!-- Slide 1 -->
        <div class="carousel-slide active">
            <img src="https://snipboard.io/6R3jOh.jpg" alt="Image 1">
        </div>
        
        <!-- Slide 2 -->
        <div class="carousel-slide">
            <img src="https://snipboard.io/6R3jOh.jpg" alt="Image 2">
        </div>
        
        <!-- Slide 3 -->
        <div class="carousel-slide">
            <img src="https://snipboard.io/6R3jOh.jpg" alt="Image 3">
        </div>
        
        <!-- Slide 4 -->
        <div class="carousel-slide">
            <img src="https://snipboard.io/6R3jOh.jpg" alt="Image 4">
        </div>
        
        <!-- Navigation Arrows -->
        <button class="carousel-arrow prev">&#10094;</button>
        <button class="carousel-arrow next">&#10095;</button>
    </div>
    
    <!-- Dots Indicator -->
    <div class="carousel-dots">
        <span class="carousel-dot active" data-index="0"></span>
        <span class="carousel-dot" data-index="1"></span>
        <span class="carousel-dot" data-index="2"></span>
        <span class="carousel-dot" data-index="3"></span>
    </div>
</div>

<br>

<p>Lorem link</p>

<script>
// Carousel functionality for both carousels
document.addEventListener('DOMContentLoaded', function() {
    // Initialize first carousel
    initCarousel('isolated-carousel');
    
    // Initialize second carousel  
    initCarousel('isolated-carousel-2');
    
    function initCarousel(carouselId) {
        const carousel = document.getElementById(carouselId);
        
        if (!carousel) {
            console.log('Carousel not found:', carouselId);
            return;
        }
        
        const slides = carousel.querySelectorAll('.carousel-slide');
        const dots = carousel.querySelectorAll('.carousel-dot');
        const prevBtn = carousel.querySelector('.carousel-arrow.prev');
        const nextBtn = carousel.querySelector('.carousel-arrow.next');
        
        if (slides.length === 0) {
            console.log('No slides found in carousel:', carouselId);
            return;
        }
        
        let currentSlide = 0;
        const totalSlides = slides.length;
        
        function showSlide(index) {
            // Ensure index is within bounds
            if (index < 0) index = totalSlides - 1;
            if (index >= totalSlides) index = 0;
            
            slides.forEach(slide => {
                slide.classList.remove('active');
            });
            
            dots.forEach(dot => {
                dot.classList.remove('active');
            });
            
            slides[index].classList.add('active');
            if (dots[index]) {
                dots[index].classList.add('active');
            }
            
            currentSlide = index;
        }
        
        function nextSlide() {
            let nextIndex = currentSlide + 1;
            if (nextIndex >= totalSlides) {
                nextIndex = 0;
            }
            showSlide(nextIndex);
        }
        
        function prevSlide() {
            let prevIndex = currentSlide - 1;
            if (prevIndex < 0) {
                prevIndex = totalSlides - 1;
            }
            showSlide(prevIndex);
        }
        
        if (nextBtn) nextBtn.addEventListener('click', nextSlide);
        if (prevBtn) prevBtn.addEventListener('click', prevSlide);
        
        dots.forEach(dot => {
            dot.addEventListener('click', function() {
                const slideIndex = parseInt(this.getAttribute('data-index'));
                if (!isNaN(slideIndex)) {
                    showSlide(slideIndex);
                }
            });
        });
        
        // Auto-advance slides
        let slideInterval = setInterval(nextSlide, 5000);
        
        const carouselSlides = carousel.querySelector('.carousel-slides');
        if (carouselSlides) {
            carouselSlides.addEventListener('mouseenter', () => {
                clearInterval(slideInterval);
            });
            
            carouselSlides.addEventListener('mouseleave', () => {
                slideInterval = setInterval(nextSlide, 5000);
            });
            
            // Touch swipe support
            let startX = 0;
            let endX = 0;
            
            carouselSlides.addEventListener('touchstart', (e) => {
                startX = e.touches[0].clientX;
            });
            
            carouselSlides.addEventListener('touchend', (e) => {
                endX = e.changedTouches[0].clientX;
                handleSwipe();
            });
            
            function handleSwipe() {
                const swipeThreshold = 50;
                
                if (startX - endX > swipeThreshold) {
                    nextSlide();
                } else if (endX - startX > swipeThreshold) {
                    prevSlide();
                }
            }
        }
        
        // Initialize first slide
        showSlide(0);
    }
});
</script>