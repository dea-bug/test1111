---
layout: page
title: Testimonials
permalink: /testimonials
---
- put widget on top, fix styling so the header isn't changed, make it hold longer text, make it mobile friendly text size
<style>
/* Testimonial CSS Code Start */
/* background */
.carousel-bg {
  background-color: none;
  margin-top: 40px;
  margin-bottom: 40px;
}
/* quote */
.quote-image {
  margin-left: auto;
  margin-right: auto;
  margin-bottom: auto;
  padding-top: 60px;
  width: 80px;
}
/* text-style */
.testimonial-style .testimonial-caption-style {
  font-family: "Roboto";
  font-weight: 400;
  font-size: 24px;
  color: #354052;
  line-height: 30px;
  bottom: 40%;
  text-shadow: none;
  top: 10%;
}
.testimonial-style .testimonial-authors {
  font-family: "Roboto";
  font-weight: 700;
  font-size: 20px;
  color: #354052;
  line-height: 30px;
  margin-top: 40px;
}
/* carousel-height-control */
.testimonial-style .carousel-inner > .item {
  padding-top: auto;
  padding-bottom: auto;
  height: 600px;
}
/* carousel-left-right-control */
.testimonial-style .carousel-control.left {
  background: none;
  box-shadow: none;
  text-shadow: none;
}
.testimonial-style .carousel-control.right {
  background: none;
  box-shadow: none;
  text-shadow: none;
}
.testimonial-style .carousel-control {
  color: #354052;
}
.testimonial-style .carousel-control:hover {
  color: #354052;
  text-decoration: none;
  transition: background-color 1s ease;
}
/* indicators */
.testimonial-style .carousel-indicators .active {
  background-color: #fff;
  width: 14px;
  height: 14px;
  transition: background 1s cubic-bezier(0.22, 0.61, 0.36, 1);
}
.testimonial-style .carousel-indicators li {
  border: 2px solid #354052;
  background-color: #354052;
}
/* Textimonial CSS Code End */
</style>

<head>
  <meta charset="UTF-8">
  <title>Bootstrap 3 Carousel Custom</title>
  <!-- CSS and JS file -->
  <link rel="stylesheet" href="https://netdna.bootstrapcdn.com/bootstrap/3.0.3/css/bootstrap.min.css">
  <link rel="stylesheet" href="https://netdna.bootstrapcdn.com/bootstrap/3.0.3/css/bootstrap-theme.min.css">
  <script type="text/javascript" src="https://code.jquery.com/jquery.min.js"></script>
  <script src="https://netdna.bootstrapcdn.com/bootstrap/3.0.3/js/bootstrap.min.js"></script>
  <!-- CSS and JS file end here -->
</head>

<body class="carousel-bg">
  <!-- Quote Image -->
  <div>
    <img src="https://i.imgur.com/gZ5HY0U.png" class="img-responsive quote-image">
  </div>
  <!-- Carousel Start below -->
  <div id="carousel1" class="carousel slide testimonial-style" data-ride="carousel">
    <!-- Indicators -->
    <ol class="carousel-indicators">
      <li data-target="#carousel1" data-slide-to="0" class="active"></li>
      <li data-target="#carousel1" data-slide-to="1"></li>
      <li data-target="#carousel1" data-slide-to="2"></li>
    </ol>
    <!-- Wrapper for slides -->
    <div class="carousel-inner">
      <div class="item active">
        <div class="carousel-caption testimonial-caption-style">
          <p>Powerful work. Great storytellers.</p>
          <p class="testimonial-authors">Craig Zablocki | Keynote & Motivational Speaker </b><br> //craigzablocki.com </p></p>
        </div>
      </div>
      <div class="item">
        <div class="carousel-caption testimonial-caption-style">
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Vitae semper quis lectus nulla at volutpat diam.</p>
          <p class="testimonial-authors">Person 2</p>
        </div>
      </div>
      <div class="item">
        <div class="carousel-caption testimonial-caption-style">
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Vitae semper quis lectus nulla at volutpat diam.</p>
          <p class="testimonial-authors">Person 3</p>
        </div>
      </div>
    </div>

    <!-- Controls -->

    <a class="left carousel-control" href="#carousel1" data-slide="prev"> <span class="glyphicon glyphicon-chevron-left"></span> </a>
    <a class="right carousel-control" href="#carousel1" data-slide="next"> <span class="glyphicon glyphicon-chevron-right"></span> </a>
  </div>
</body>

<br>
<p><em>"We were new to shooting videos, Deana and Aster walked us patiently and carefully through the process, beautifully edited our footage and gave us a finished product to be proud of! We especially appreciate how they kept to schedule with such professionalism. We’re excited to work with them again on other projects!"</em>
<br><b>Diana Horowitz & Amelia Vargas | EastWest Microneedling, LLC </b><br> //www.eastwestmicroneedling.com </p>
<br>
<p><em>"Super easy to work with! I loved how our fundraiser video came out."</em>
<br><b>Carly Stoliker | Development Manager at LAWs </b><br> //www.lcsj.org </p>
<br>
<p><em>"Powerful work. Great storytellers."</em>
<br><b>Craig Zablocki | Keynote & Motivational Speaker </b><br> //craigzablocki.com </p>

<br>