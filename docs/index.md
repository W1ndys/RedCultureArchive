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
        <img src="slide1.jpg" alt="Slide 1">
    </div>

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


</script>

<div class="grid cards" markdown>
<div class="grid cards" markdown>
- [红船精神](/RedShipMind/ )

- [井冈山精神](/JinggangshanMind/)

- [长征精神](/ChangzhengMind/)

- [延安精神](/YananMind/)

- [西柏坡精神](/XibopuMind/)

</div>

</div>

<div class="grid cards" markdown>
<div class="grid cards" markdown>
-   每月推荐:

    ---

    ![青岛](qingdao.jpg)

</div>

<div class="grid cards" markdown>
- 地图:点击可直接跳转百度地图搜索四川省

    ---

    [![map](map.jpg)](https://map.baidu.com/search/%E5%9B%9B%E5%B7%9D%E7%9C%81/@11202974.97015903,3516933.635000112,7.66z?querytype=s&da_src=shareurl&wd=%E5%9B%9B%E5%B7%9D&c=286&src=0&pn=0&sug=0&l=13&b=(12954181,4167162;13015621,4196570)&from=webmap&biz_forward=%7B%22scaler%22:1,%22styles%22:%22pl%22%7D&device_ratio=1){target="_blank"}

</div>

</div>
