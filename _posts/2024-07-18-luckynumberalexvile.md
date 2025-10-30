---
layout: post
title: "Alex Vile - Lucky Number"
author: "Deana Seitz and Aster Teter"
categories: music videos
tags: [music videos, color grading]
image: luckynumber.jpg
---

<!-- First Carousel -->
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

<!-- Second Carousel -->
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

Lorem link

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