---
title: 首页
comments: true
hide:
  - tags
  - navigation
  - footer
  - toc
  - actions
---

<style>
    .slideshow-container {
        max-width: 600px;
        position: relative;
        margin: auto;
    }

    .slide {
        display: none;
    }

    .slide img {
        width: 100%;
        height: auto;
    }

    .prev, .next {
        position: absolute;
        top: 50%;
        transform: translateY(-50%);
        cursor: pointer;
        padding: 16px;
        color: white;
        font-weight: bold;
        font-size: 20px;
        z-index: 1;
        background-color: rgba(0, 0, 0, 0.5);
        border: none;
    }

    .prev {
        left: 0;
    }

    .next {
        right: 0;
    }
</style>

<div class="slideshow-container">
    <div class="slide">
        <img src="slide1.png" alt="Slide 1">
    </div>
    <div class="slide">
        <img src="slide2.png" alt="Slide 2">
    </div>
    <div class="slide">
        <img src="slide3.png" alt="Slide 3">
    </div>

    <button class="prev" onclick="plusSlides(-1)">❮</button>
    <button class="next" onclick="plusSlides(1)">❯</button>

</div>

<script>
    let slideIndex = 1;
    showSlides(slideIndex);

    function plusSlides(n) {
        showSlides(slideIndex += n);
    }

    function currentSlide(n) {
        showSlides(slideIndex = n);
    }

    function showSlides(n) {
        let i;
        const slides = document.getElementsByClassName("slide");
        if (n > slides.length) {slideIndex = 1}
        if (n < 1) {slideIndex = slides.length}
        for (i = 0; i < slides.length; i++) {
            slides[i].style.display = "none";
        }
        slides[slideIndex-1].style.display = "block";
    }

    // 自动轮播
    setInterval(function() {
        plusSlides(1);
    }, 2000);
</script>

<div class="grid cards" markdown>
<div class="grid cards" markdown>
- [红船精神](/RedShipMind/ )

- [井冈山精神](/JinggangshanMind/)

- [长征精神](/ChangzhengMind/)

- [延安精神](/YananMind/)

- [西柏坡精神](/XibopuMind/)

- [其他精神1](/OtherMind1/)

- [其他精神2](/OtherMind2/)

- [其他精神3](/OtherMind3/)

- [其他精神4](/OtherMind4/)

</div>

</div>

<div class="grid cards" markdown>
<div class="grid cards" markdown>
-   每月推荐:

    ---

    - [五四青年节](/54/ )

    - [推荐2](/recommend2/)

    - [推荐3](/recommend3/)

    - [推荐4](/recommend4/)

    - [推荐5](/recommend5/)

</div>

<div class="grid cards" markdown>
-   推荐工具:

    ---

    - [高德地图](https://www.amap.com/)

    - [百度地图](https://map.baidu.com/)

    - [腾讯地图](https://map.qq.com/)

    - [搜狗地图](https://map.sogou.com/)

    - [谷歌地图](https://www.google.com/maps/)

</div>

</div>
