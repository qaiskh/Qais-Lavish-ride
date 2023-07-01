<template>
    <div style="padding: 0rem 5rem;">

        <div style="display: flex; align-items: center; ">
            <div class="slider-icon2">
                <v-icon style="font-size: 30px;" color="#ffe09e" icon="mdi-clipboard-list-outline"></v-icon>
            </div>
            <div>
                <h3 style="color:#6e5596">Try Our Healthy Menu</h3>
            </div>

        </div>

        

        <div>
            <div class="value-span-section2" style="display: flex; align-items: center;">
                We provide a Variety of healthy recipes that have been curated by our best nutritionists for you
            </div>

        </div>
        <div style="display: flex; justify-content: flex-end;">
            <div class="icon-container2">
                <v-icon style="font-size: 30px;" id="prev-button" color="grey" icon="mdi-chevron-left"></v-icon>
            </div>
            <div class="icon-container2">
                <v-icon style="font-size: 30px;" id="next-button" color="grey" icon="mdi-chevron-right"></v-icon>
            </div>

        </div>
    </div>
    <div style="height: 65vh;">
        <div class="main-container5" style="display: flex;">
            <div class="wrapper" style="width: 40%; padding: 2rem 4rem;">
                <ul class="test">
                    <li>
                        <div class="menu-card2">
                            <div class="menu-icon">
                                <v-icon style="font-size: 30px;" color="#ffff" icon="mdi-clock-outline"></v-icon>
                            </div>
                            <div>
                                <h3 style="color:#965af9">Try Our Healthy Menu</h3>
                            </div>

                        </div>
                    </li>
                    <li>
                        <div class="menu-card2">
                            <div class="menu-icon-goald">
                                <v-icon class="gold-icon" style="font-size: 30px;" color="#ffff"
                                    icon="mdi-send-outline"></v-icon>
                            </div>
                            <div>
                                <h3 style="color:#965af9">Try Our Healthy Menu</h3>
                            </div>

                        </div>
                    </li>
                    <li>
                        <div class="menu-card2">
                            <div class="menu-icon">
                                <v-icon style="font-size: 30px;" color="#ffff" icon="mdi-calendar-month"></v-icon>
                            </div>
                            <div>
                                <h3 style="color:#965af9">Try Our Healthy Menu</h3>
                            </div>

                        </div>
                    </li>
                    <li>
                        <div class="menu-card2">
                            <div class="menu-icon">
                                <v-icon style="font-size: 30px;" color="#ffff" icon="mdi-lock"></v-icon>
                            </div>
                            <div>
                                <h3 style="color:#965af9">Try Our Healthy Menu</h3>
                            </div>

                        </div>
                    </li>
                    <li>
                        <div class="menu-card2">
                            <div class="menu-icon">
                                <v-icon style="font-size: 30px;" color="#ffff" icon="mdi-calendar-month"></v-icon>
                            </div>
                            <div>
                                <h3 style="color:#965af9">Try Our Healthy Menu</h3>
                            </div>

                        </div>
                    </li>
                </ul>
            </div>
            <div class="slider-section" style="width: 60%;">
                <div class="carousel-container2">
                    <div class="carousel-wrapper">
                        <div class="carousel">
                            <div class="card2">
                                <div class="half-circle">
                                    <div class="content">
                                        <img class="image-section1" style="width: 100%; height: 100%; margin-right: 15px;" src="/public/png2.png"
                                            alt="" />
                                    </div>

                                </div>
                                <div class="slider-text">
                                    <h4 style=" margin-block-start: 15px; color: #69548e;"> Healthy Recipe</h4>
                                    <button class="slider-btn">Try Now</button>
                                </div>

                            </div>
                            <div class="card2">
                                <div class="half-circle">
                                    <div class="content">
                                        <img class="image-section1" style="width: 100%; height: 100%; margin-right: 15px;" src="/public/png2.png"
                                            alt="" />
                                    </div>

                                </div>
                                <div class="slider-text">
                                    <h4 style=" margin-block-start: 15px; color: #69548e;"> Healthy Recipe</h4>
                                    <button class="slider-btn">Try Now</button>
                                </div>

                            </div>
                            <div class="card2">
                                <div class="half-circle">
                                    <div class="content">
                                        <img class="image-section1" style="width: 100%; height: 100%; margin-right: 15px;" src="/public/png2.png"
                                            alt="" />
                                    </div>

                                </div>
                                <div class="slider-text">
                                    <h4 style=" margin-block-start: 15px; color: #69548e;"> Healthy Recipe</h4>
                                    <button class="slider-btn">Try Now</button>
                                </div>

                            </div>
                            <div class="card2">
                                <div class="half-circle">
                                    <div class="content">
                                        <img class="image-section1" style="width: 100%; height: 100%; margin-right: 15px;" src="/public/png2.png"
                                            alt="" />
                                    </div>

                                </div>
                                <div class="slider-text">
                                    <h4 style=" margin-block-start: 15px; color: #69548e;"> Healthy Recipe</h4>
                                    <button class="slider-btn">Try Now</button>
                                </div>

                            </div>
                            <div class="card2">
                                <div class="half-circle">
                                    <div class="content">
                                        <img class="image-section1" style="width: 100%; height: 100%; margin-right: 15px;" src="/public/png2.png"
                                            alt="" />
                                    </div>

                                </div>
                                <div class="slider-text">
                                    <h4 style=" margin-block-start: 15px; color: #69548e;"> Healthy Recipe</h4>
                                    <button class="slider-btn">Try Now</button>
                                </div>

                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </div>
</template>
<script setup>
import { onMounted } from 'vue'

// JavaScript logic
let container
let itemsContainer
let items
let itemWidth
let currentPosition = 0

// Initialize the carousel
onMounted(() => {
    const prevButton = document.getElementById('prev-button');
    const nextButton = document.getElementById('next-button');
    const carousel = document.querySelector('.carousel-wrapper');

    prevButton.addEventListener('click', () => {
        carousel.scrollBy({
            left: -carousel.offsetWidth,
            behavior: 'smooth'
        });
    });

    nextButton.addEventListener('click', () => {
        carousel.scrollBy({
            left: carousel.offsetWidth,
            behavior: 'smooth'
        });
    });
})

// Function to scroll the carousel
function scrollCarousel(direction) {
    if (direction === 'prev') {
        currentPosition -= itemWidth
    } else {
        currentPosition += itemWidth
    }

    currentPosition = Math.max(
        0,
        Math.min(
            currentPosition,
            itemsContainer.offsetWidth - container.offsetWidth,
        ),
    )

    itemsContainer.style.transform = `translateX(${-currentPosition}px)`
}
</script>
<style lang="scss">
.value-span-section2 {
    margin-block-start: 25px;
    width: 28%;
    color: #a6a0b9;
}


ul {
    width: 400px;
    max-height: 450px;
    overflow-x: hidden;
    overflow-y: auto;
    scrollbar-width: thin;
    scrollbar-color: #6969dd #e0e0e0;
}

.test {
    scrollbar-width: thin;
    scrollbar-color: #6969dd #e0e0e0;
}

.test::-webkit-scrollbar {
    width: 10px;
}

.test::-webkit-scrollbar-track {
    background-color: darkgrey;
}

ul {
    margin: 1em;
    color: white;
    font-family: sans-serif;
    font-size: 16px;
}

li {
    padding: 1em;

    ul {
        margin: 0;
    }

    .wrapper {
        cursor: auto;

        li {
            padding: 0.5em;
        }
    }

    &.parent {

        cursor: pointer;
    }
}

.menu-icon {
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
    border-radius: 10px;
    padding: 10px;
    background-color: #965af9;
    margin-inline-end: 15px;
    margin-inline-start: 10px;
}

.menu-icon-goald {
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
    border-radius: 10px;
    padding: 10px;
    background-color: #ffbf1f;
    margin-inline-end: 15px;
    margin-inline-start: 10px;
}

.menu-card2 {
    display: flex;
    align-items: center;
    border-radius: 25px;
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
    height: 11vh;
    background-color: #f9f1fe;
}

.gold-icon {
    transform: rotate(45deg);
}


.half-circle {
    width: 200px;
    height: 200px;
    border: 9px solid #fbf8f8;
    border-radius: 100px 100px 20px 20px;
    background-color: #9d9be5;
    position: relative;
    display: flex;
    align-items: center;
    padding-left: 20px;
    overflow: hidden;
    margin-block-start: 9px;
}

.content {
    padding: 10px;
}

.carousel-container2 {
    width: 89%;
    overflow: hidden;
    position: relative;
}

.carousel-wrapper {
    display: flex;
    overflow-x: inherit;
    scroll-behavior: smooth;
    -webkit-overflow-scrolling: touch;
}

.slider-section {
    width: 60%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.carousel {
    display: flex;
}

.card2 {
    width: 300px;
    height: 350px;
    margin-right: 10px;
    padding-block-start: 21px;
    margin-left: 70px;
    color: #69548e;
    border-radius: 100px 100px 0 0;
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
    position: relative;
    overflow: hidden;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}


.content{
    display: flex;
    justify-content: center;
    align-items: center;
    margin-right: 17px;
}
.slider-btn {
    background: #fed165;
    font-size: 15px;
    padding: 10px 3px;
    margin-block-start: 20px;
    width: 100%;
    color: black;
    border-radius: 12px;
    border: 3px solid #fdf2d6;
}
.slider-text{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
</style>