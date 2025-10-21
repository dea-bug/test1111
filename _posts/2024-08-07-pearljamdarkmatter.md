---
layout: post
author: "Deana Seitz and Aster Teter"
title: "Pearl Jam: Dark Matter World Tour 2024"
categories: music videos
tags: [music videos, color grading, editing, visuals]
image: pjdm-header.jpg
---
<!-- make modals stack horizonally on mobile, increase modal size, make image with blurb, check if montserrat, change the white flash on slide(?), add credits at bottom of page? -->
<!-- Header Animation -->
<div class="anim-header-container">
    <div class="anim-image-wrapper">
        <img src="https://joybirdstudios.com/assets/img/darkmatter-header.jpg" alt="Animated concert ticket header image"> 
        <div class="anim-title-container">
            <span class="anim-title-line">Pearl Jam: Dark Matter</span>
            <span class="anim-title-line">World Tour 2024</span>
        </div>
    </div>
</div>

<!-- Photo credit -->
<link href="https://fonts.googleapis.com/css2?family=Anton&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css?family=Raleway|Rozha+One" rel="stylesheet">

<style>
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

/* Gallery Styles */
.gallery-container {
    --gallery-primary-color: #fff;
    --gallery-secondary-color: rgba(0, 0, 0, 0.9);
    --gallery-transition-duration: 0.5s;
    margin-bottom: 40px;    
    padding: 0px;
    background: #fff;
}

.gallery-container .col4 {
    width: 31%;
    float: left;
    position: relative;
}

.gallery-container .transition {
    transition: all var(--gallery-transition-duration) ease;
}

.gallery-container .container {
    width: 118%;
    margin: 0 auto;
    overflow: hidden;
}

.gallery-container .fx2 .item {
    margin: 4px;
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

/* Modal Styles */
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

.gallery-container .close-button {
    height: 50px;
    width: 50px;
    position: fixed;
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

.gallery-container #close {
    display: none;
}

/* Carousel Styles */
#isolated-carousel {
    all: initial;
    display: block;
    max-width: 900px;
    margin: 20px auto;
    padding: 20px;
    position: relative;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

#isolated-carousel .carousel-slides {
    all: initial;
    display: block;
    position: relative;
    height: 500px;
    overflow: hidden;
    border-radius: 8px;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
    box-sizing: border-box;
}

#isolated-carousel .carousel-slide {
    all: initial;
    display: block;
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
    opacity: 1;
}

#isolated-carousel .carousel-slide img {
    all: initial;
    display: block;
    max-width: 100%;
    max-height: 100%;
    width: auto;
    height: auto;
    object-fit: contain;
    box-sizing: border-box;
}

#isolated-carousel .carousel-arrow {
    all: initial;
    display: block;
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
    all: initial;
    display: flex;
    justify-content: center;
    margin-top: 20px;
    gap: 10px;
    box-sizing: border-box;
}

#isolated-carousel .carousel-dot {
    all: initial;
    display: block;
    width: 12px;
    height: 12px;
    border-radius: 50%;
    background-color: #ccc;
    cursor: pointer;
    transition: background-color 0.3s;
    box-sizing: border-box;
}

#isolated-carousel .carousel-dot.active {
    background-color: #333;
}

/* Second Carousel Styles */
#isolated-carousel-2 {
    all: initial;
    display: block;
    max-width: 900px;
    margin: 20px auto;
    padding: 20px;
    position: relative;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

#isolated-carousel-2 .carousel-slides {
    all: initial;
    display: block;
    position: relative;
    height: 500px;
    overflow: hidden;
    border-radius: 80px;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
    box-sizing: border-box;
}

#isolated-carousel-2 .carousel-slide {
    all: initial;
    display: block;
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
    opacity: 1;
}

#isolated-carousel-2 .carousel-slide img {
    all: initial;
    display: block;
    max-width: 100%;
    max-height: 100%;
    width: auto;
    height: auto;
    object-fit: contain;
    box-sizing: border-box;
}

#isolated-carousel-2 .carousel-arrow {
    all: initial;
    display: block;
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
    all: initial;
    display: flex;
    justify-content: center;
    margin-top: 20px;
    gap: 10px;
    box-sizing: border-box;
}

#isolated-carousel-2 .carousel-dot {
    all: initial;
    display: block;
    width: 12px;
    height: 12px;
    border-radius: 50%;
    background-color: #ccc;
    cursor: pointer;
    transition: background-color 0.3s;
    box-sizing: border-box;
}

#isolated-carousel-2 .carousel-dot.active {
    background-color: #333;
}

/* Mobile Responsiveness */
@media (max-width: 768px) {
    .anim-title-container {
        bottom: 15px;
        left: 15px;
    }
    
    .anim-title-line {
        margin-bottom: 3px;
    }
    
    .gallery-container .col4 {
        width: 50%;
    }
    
    .gallery-container .close-button {
        right: 0;
        top: -70px;
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
    
    .gallery-container .modal-image {
        max-height: 70vh;
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
<style>
font-family: 'Montserrat', sans-serif;
</style>

<p>In the winter of 2022, we had the exciting opportunity to collaborate on visuals for Pearl Jam's 2024 Dark Matter World Tour. We joined an amazing creative team led by Creative Director Rob Sheridan and Producer Stephanie Sheridan.</p>
<br>
<img src="https://snipboard.io/Gf2r7H.jpg" alt="image showing the sun projected on a screen behind Pearl Jam with text to the right text that reads: 200+ hours
of 1000 FPS super slow-motion macro footage, real NASA visuals, and archival material combined to create a captivating experience on a 155-foot screen"> 
<p>The concept for the project was to create something cosmic and awe inspiring, yet human. To bring this vision to life, we developed innovative techniques, including a custom process that allowed Rob Sheridan and his team to paint with light—typically only possible within the realm of still photography—to craft a vast organic cosmic structure for the opening track of the album, “Scared of Fear.”</p>

<!-- Carousel -->
<div id="isolated-carousel-2">
    <div class="carousel-slides">
        <!-- Slide 1 -->
        <div class="carousel-slide active">
            <img src="[link]" alt="Image 1">
        </div>
        
        <!-- Slide 2 -->
        <div class="carousel-slide">
            <img src="[link]" alt="Image 2">
        </div>
        
        <!-- Slide 3 -->
        <div class="carousel-slide">
            <img src="[link]" alt="Image 3">
        </div>
        
        <!-- Slide 4 -->
        <div class="carousel-slide">
            <img src="[link]" alt="Image 4">
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
<p>Rob Sheridan envisioned a look that was analog, organic and human rather than the typical sharp aesthetics of concert LED screens. This led us to create a soft, glowing appearance that reflected the feel and texture of film.
</p>
<p>We combined over 200 hours of 1000 FPS super slow-motion macro footage, real NASA visuals, and archival material to create a captivating experience projected onto a 155-foot screen.
</p>
[embedded and centered instagram content 2]
<br>
</center>

<br>

<!-- Final Link -->
<p>[credits placeholder]</p>
<a href="https://pearljam.com/news/dark-matter-world-tour-2024">Pearl Jam Dark Matter Tour</a>

<script>
// Carousel functionality for both carousels
document.addEventListener('DOMContentLoaded', function() {
    // Initialize first carousel
    initCarousel('isolated-carousel');
    
    // Initialize second carousel  
    initCarousel('isolated-carousel-2');
    
    function initCarousel(carouselId) {
        const carousel = document.getElementById(carouselId);
        
        if (!carousel) return;
        
        const slides = carousel.querySelectorAll('.carousel-slide');
        const dots = carousel.querySelectorAll('.carousel-dot');
        const prevBtn = carousel.querySelector('.carousel-arrow.prev');
        const nextBtn = carousel.querySelector('.carousel-arrow.next');
        
        let currentSlide = 0;
        const totalSlides = slides.length;
        
        function showSlide(index) {
            slides.forEach(slide => {
                slide.classList.remove('active');
            });
            
            dots.forEach(dot => {
                dot.classList.remove('active');
            });
            
            slides[index].classList.add('active');
            dots[index].classList.add('active');
            
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
                showSlide(slideIndex);
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
    }
});
</script>