---
layout: post
title: "The Residences at Rainier Square | Seattle WA Apartments"
author: "Deana Seitz"
categories: advertisement 
tags: [color grading, editing]
image: rainiersquare.jpeg
---
<div class="browser" url="https://www.example.org/">
    <div class="iframe-wrapper">
      <iframe src="https://www.example.org/" frameborder="0">      
      </iframe>
    </div>
</div>

<style>
html,body {
  margin: 0;
  padding: 0;
}
// credit to nikkk-me for the browser mockup
* {
  box-sizing: border-box;
}

$red: #EB7061;
$yellow: #F5D160;
$green: #81D982;
$grey: #efefef;
$white: #ffffff;
$black: #333333;

$bigDotSize: 6px;
$smallDotSize: 2px;

//background
body {
  -webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
  font-family: sans-serif;
  background: white;
  color: $black;
  font-weight: 300;
  font-size: 14px;
}

.browser {
  position: relative;
  background: white;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15), 0 6px 10px rgba(0, 0, 0, 0.1);
  min-height: 500px;
  max-width: 80%;
  margin: auto;
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
  padding-top: 45px;
  background-image: radial-gradient(circle, $red $bigDotSize, transparent $bigDotSize),radial-gradient(circle, $yellow $bigDotSize, transparent $bigDotSize),radial-gradient(circle, $green $bigDotSize, transparent $bigDotSize), radial-gradient(circle, darken($grey, 12%) $smallDotSize, transparent $smallDotSize),radial-gradient(circle, darken($grey, 12%) $smallDotSize, transparent $smallDotSize),radial-gradient(circle, darken($grey, 12%) $smallDotSize, transparent $smallDotSize), linear-gradient(to bottom, $grey 45px, transparent 0);
  background-position:  left top, left top, left top, right top, right top, right top, 0 0;
  background-size:  50px 45px, 90px 45px, 130px 45px, 50px 30px, 50px 45px, 50px 60px, 100%;
  background-repeat: no-repeat, no-repeat;

  &[url]:after {
    content: attr(url);
    color: darken($grey, 30%);
    font-size: 13px;
    font-weight: 400;
    position: absolute;
    left: 0;
    right: 0;
    top: 0;
    padding: 6px 15px;
    margin: 9px 50px 0 90px;
    border-radius: 25px;
    background: $white;
    height: 27px;
    box-sizing: border-box;
  }
}

.iframe-wrapper {
  position: relative;
  overflow: hidden;
  padding-top: 56.25%;
  
  iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border: 0;
  }
}
</style>

https://liverainiersquare.com/

Lead Editor: Deana Seitz
<br>
Colorist: Aster Teter