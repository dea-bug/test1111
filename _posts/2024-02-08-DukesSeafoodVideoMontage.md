---
layout: post
title: "Duke's Seafood | Landing Page Montage"
author: "Deana Seitz and Aster Teter"
categories: advertisement 
tags: [color grading, editing]
image: dukes2024.png
---
<!-- Header Animation -->
<div class="anim-header-container">
    <div class="anim-image-wrapper">
        <img src="https://joybirdstudios.com/assets/img/darkmatter-header.jpg" alt="Animated concert ticket header image for Pearl Jam Dark Matter tour visuals"> 
        <div class="anim-title-container">
            <span class="anim-title-line">Pearl Jam</span>
            <span class="anim-title-line">World Tour 2024</span>
        </div>
    </div>
</div>

<!-- Photo credit -->
<p style="font-size: 12px; color: grey; text-align: right; margin-top: 5px;">photos + BTS footage by <a href="https://www.rob-sheridan.com/pearl-jam-2024/dark-matter-tour/4/thumbs" target="_blank" Lorem Link>
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

/* Responsive single image in content section */
.content-single-image {
    width: 100%;
    max-width: 100%;
    height: auto;
    display: block;
    margin: 20px 0;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

/* Gallery Styles */
.gallery-container {
    --gallery-primary-color: #fff;
    --gallery-secondary-color: rgba(0, 0, 0, 0.9);
    --gallery-transition-duration: 0.5s;
    margin-bottom: 40px;
    font-family: 'Montserrat', sans-serif;
    background: #fff;
}

.gallery-container .container {
    width: 100% !important;
    margin: 0 auto;
    overflow: hidden;
}

/* Use flexbox for horizontal stacking */
.gallery-container .fx2 {
    display: flex !important;
    flex-direction: row !important;
    flex-wrap: nowrap !important;
    justify-content: space-between !important;
    align-items: stretch !important;
    width: 100% !important;
    gap: 1px !important;
}

.gallery-container .col4 {
    flex: 1 !important;
    min-width: 0 !important; /* Allow flex items to shrink */
    position: relative;
    box-sizing: border-box;
}

.gallery-container .transition {
    transition: all var(--gallery-transition-duration) ease;
}

.gallery-container .fx2 .item {
    margin: 0 !important;
    padding: 0;
    cursor: pointer;
    overflow: hidden;
    width: 100%;
    height: 100%;
}

.gallery-container .fx2 .item img {
    padding: 0 !important;
    display: block;
    max-width: 100%;
    height: auto;
    width: 100%;
    object-fit: cover;
    aspect-ratio: 1 / 1; /* Ensure consistent sizing */
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
    z-index: 10000;
    pointer-events: none;
    padding: 10px;
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
    max-width: 95% !important;
    max-height: 95% !important;
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
    max-height: 85vh !important;
    height: auto;
    display: block;
    margin: 0 auto;
}

.gallery-container .close-button {
    height: 50px;
    width: 50px;
    position: fixed;
    top: 20px !important;
    right: 20px !important;
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
    border-radius: 80px;
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
    background-color: black;
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
    background-color: rgba(0, 0, 0, 0.8);
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

/* Mobile Responsiveness */
@media (max-width: 768px) {
    
    #isolated-carousel .carousel-slides {
        height: 350px;
    }
    
    #isolated-carousel .carousel-arrow {
        width: 40px;
        height: 40px;
        font-size: 20px;
    }
}

@media (max-width: 480px) {

    #isolated-carousel .carousel-slides {
        height: 250px;
    }
    
    #isolated-carousel .carousel-arrow {
        width: 35px;
        height: 35px;
        font-size: 18px;
    }
    
    #isolated-carousel .carousel-dot {
        width: 12px;
        height: 12px;
    }
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
    
    /* Keep horizontal layout on tablet but adjust spacing */
    
    .gallery-container .close-button {
        right: 10px !important;
        top: 10px !important;
    }
    
    .gallery-container .modal-content {
        max-width: 98% !important;
        max-height: 98% !important;
    }
}

@media (max-width: 480px) {
    .anim-title-container {
        bottom: 10px;
        left: 10px;
        width: 80%;
    }
    
    
    /* Ensure single image is fully responsive on mobile */
    .content-single-image {
        max-width: 100% !important;
        height: auto !important;
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
                    <img class="transition img-responsive" src="https://joybirdstudios.com/assets/img/Climate-Pledge-Rehearsals.jpg" alt="Gallery image 1">
                </div>
            </a>
            
            <!-- Image 2 -->
            <a href="#image2" class="image-link">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://joybirdstudios.com/assets/img/Climate-Pledge-Rehearsals.jpg" alt="Gallery image 2">
                </div>
            </a>
            
            <!-- Image 3 -->
            <a href="#image3" class="image-link">
                <div class="item col4">
                    <img class="transition img-responsive" src="https://joybirdstudios.com/assets/img/ClimatePledgeRehearsals3.jpg" alt="Gallery image 3">
                </div>
            </a>
        </div>

        <!-- Gallery Modals -->
        <div class="modal" id="image1">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://joybirdstudios.com/assets/img/Climate-Pledge-Rehearsals.jpg" class="modal-image" alt="Modal image 1">
                <a href="#" class="close-button"></a>
            </div>
        </div>

        <div class="modal" id="image2">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://joybirdstudios.com/assets/img/Climate-Pledge-Rehearsals.jpg" class="modal-image" alt="Modal image 2">
                <a href="#" class="close-button"></a>
            </div>
        </div>

        <div class="modal" id="image3">
            <a href="#" class="modal-close"></a>
            <div class="modal-content">
                <img src="https://joybirdstudios.com/assets/img/ClimatePledgeRehearsals3.jpg" class="modal-image" alt="Modal image 3">
                <a href="#" class="close-button"></a>
            </div>
        </div>

        <div id="close"></div>
    </div>
</div>

<!-- Content Sections -->
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Vitae semper quis lectus nulla at volutpat diam</p>
<br>

<!-- Responsive Single Image -->
<img src="https://snipboard.io/6R3jOh.jpg" alt="Content image" class="content-single-image">

<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Vitae semper quis lectus nulla at volutpat diam</p>

<br>

<!-- More Content -->
<center>
<p>Take a glimpse of our process below:</p>
<br>
[embedded and centered instagram content 1]
</center>
<br>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Vitae semper quis lectus nulla at volutpat diam</p>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Vitae semper quis lectus nulla at volutpat diam</p>
<center>
[embedded and centered instagram content 2]
</center>
<br>
<!-- Carousel -->
<div id="isolated-carousel">
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
<a href="https://pearljam.com/news/dark-matter-world-tour-2024" target="_blank">


  Pearl Jam Dark Matter World Tour 2024


</a>


<p>


<script>
document.addEventListener('DOMContentLoaded', function() {

    initCarousel('isolated-carousel');
    
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