---
layout: default
title: Home
---

<div class="hero-section">
  <div class="slideshow-container">
    <div class="slide fade">
      <img src="{{ '/assets/images/slide1.svg' | relative_url }}" alt="Slide 1">
    </div>
    <div class="slide fade">
      <img src="{{ '/assets/images/slide2.svg' | relative_url }}" alt="Slide 2">
    </div>
    <div class="slide fade">
      <img src="{{ '/assets/images/slide3.svg' | relative_url }}" alt="Slide 3">
    </div>
    
    <a class="prev" onclick="changeSlide(-1)">&#10094;</a>
    <a class="next" onclick="changeSlide(1)">&#10095;</a>
  </div>
  
  <div class="dots-container">
    <span class="dot" onclick="currentSlide(1)"></span>
    <span class="dot" onclick="currentSlide(2)"></span>
    <span class="dot" onclick="currentSlide(3)"></span>
  </div>
</div>

<div class="content-section">
  <h2>Welcome</h2>
  <p>Hi, I'm [Your Name]. Welcome to my personal website!</p>
  <p>[Add a brief introduction about yourself, your work, and what visitors can find on your site.]</p>
  
  <div class="cta-buttons">
    <a href="{{ site.cv_link }}" class="btn btn-primary">View My CV</a>
    <a href="/about" class="btn btn-secondary">About Me</a>
  </div>
</div>

<script src="{{ '/assets/js/slideshow.js' | relative_url }}"></script>
