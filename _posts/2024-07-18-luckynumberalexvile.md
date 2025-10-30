---
layout: post
title: "Alex Vile - Lucky Number"
author: "Deana Seitz and Aster Teter"
categories: music videos
tags: [music videos, color grading]
image: luckynumber.jpg
---

<style>

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
</style>

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

Lorem link here!

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
