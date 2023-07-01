<template>
    <div class="main-container6">

        <div class="image-section">
            <img class="image-section1" src="/public/pngegg.png" alt="" />
        </div>
        <div class="value-text-section">
            <div style="display: flex; align-items: center;">
                <div class="slider-icon2">
                    <v-icon style="font-size: 30px;" color="#ffff" icon="mdi-email-open"></v-icon>
                </div>
                <div>
                    <h3>Testimonials About Us </h3>
                </div>
            </div>
            <div class="value-span-section2">
                In the smallest case we always give your best,find out what
                other users have to say about us
            </div>
            <div class="carousel-container4">
                <div class="carousel-wrapper4">

                    <div class="carousel">
                        <div class="card3">
                            <div class="slider-icon4">
                                <v-icon style="font-size: 30px;" color="#ffff" icon="mdi-message-text-outline"></v-icon>
                            </div>
                            <p>
                                "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut rutrum ultricies justo, nec
                                bibendum orci.
                                Nunc eu accumsan lorem. Nullam ac tellus ac sem congue fermentum."
                            </p>
                            <h3 style="color: #a16ff1; margin-left: 9px;">Rara Sanchez</h3>
                            <h4 style="color: #b0a5bb; margin-left: 9px;">Freelancer</h4>
                        </div>
                        <div class="card3">
                            <div class="slider-icon4">
                                <v-icon style="font-size: 30px;" color="#ffff" icon="mdi-message-text-outline"></v-icon>
                            </div>
                            <p>
                                "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut rutrum ultricies justo, nec
                                bibendum orci.
                                Nunc eu accumsan lorem. Nullam ac tellus ac sem congue fermentum."
                            </p>
                            <h3 style="color: #a16ff1; margin-left: 9px;">Rara Sanchez</h3>
                            <h4 style="color: #b0a5bb; margin-left: 9px;">Freelancer</h4>
                        </div>
                        <div class="card3">
                            <div class="slider-icon4">
                                <v-icon style="font-size: 30px;" color="#ffff" icon="mdi-message-text-outline"></v-icon>
                            </div>
                            <p>
                                "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut rutrum ultricies justo, nec
                                bibendum orci.
                                Nunc eu accumsan lorem. Nullam ac tellus ac sem congue fermentum."
                            </p>
                            <h3 style="color: #a16ff1; margin-left: 9px;">Rara Sanchez</h3>
                            <h4 style="color: #b0a5bb; margin-left: 9px;">Freelancer</h4>
                        </div>
                    </div>
                </div>
                <div class="slider-button">
                    <div class="icon-container2">
                        <v-icon style="font-size: 30px;" id="prev" color="grey" icon="mdi-chevron-left"></v-icon>
                    </div>
                    <div class="icon-container2">
                        <v-icon style="font-size: 30px;" id="next" color="grey" icon="mdi-chevron-right"></v-icon>
                    </div>
                </div>
            </div>


        </div>
    </div>
</template>
  
<script setup>
import { onMounted } from 'vue'


onMounted(() => {
    const prev = document.getElementById('prev');
    const next = document.getElementById('next');
    const carousel = document.querySelector('.carousel-wrapper4');

    prev.addEventListener('click', () => {
        carousel.scrollBy({
            left: -carousel.offsetWidth,
            behavior: 'smooth'
        });
    });

    next.addEventListener('click', () => {
        carousel.scrollBy({
            left: carousel.offsetWidth,
            behavior: 'smooth'
        });
    });
})

</script>
<style>
.image-section1 {
    width: 85%;
    height: 125%;
}

.image-section {
    justify-content: flex-end;
    display: flex;
}

.text-size {
    font-size: 24px;
}

.video-section {
    display: flex;
    align-items: center;
}

.icon-container {
    cursor: pointer;
    margin-inline: 20px;
    background-color: white;
    padding: 10px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.value-section {
    justify-content: space-between;
    display: flex;

}

.value-span-section2 {
    margin-block-start: 25px;
    padding-block-end: 25px;
    color: #a6a0b9;
    width: 400px;
}

.slider-button {
    display: flex;
    justify-content: end;
    position: inherit;
    bottom: 60px;
    right: 10px;
}

.first-btn {
    background: gold;
    font-size: 24px;
    padding: 20px 50px;
    color: black;
    border-radius: 20px;
}

.color-text {
    font-size: 100px;
    font-weight: 700;
    line-height: 110px;
}


.main-container6 {
    display: flex;
    justify-content: space-between;
    padding: 3rem 5rem;
    height: 80vh;
}

.value-text-section {
    width: 600px;
    margin: 0px;
    color: #965af9;
    font-family: 'Roboto';
}

.slider-icon3 {
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
    border-radius: 10px;
    padding: 10px;
    background-color: #965af9;
    margin-inline-end: 15px;
    position: relative;
    bottom: 40px;
    right: 76px;

}

.slider-icon4{
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
    border-radius: 10px;
    padding: 10px;
    background-color: #965af9;
    width: 50px;
    position: relative;
    bottom: 40px;
    left: 10px;
    margin-inline-end: 15px;
}

.carousel-container4 {
    width: 100%;
    overflow: hidden;
    position: relative;
}

.carousel-wrapper4 {
    display: flex;
    overflow-x: inherit;
    scroll-behavior: smooth;
}

.carousel {
    display: flex;
}

.card3 {
    width: 600px;
    height: 300px;
    background-color: #f9f1fe;
    display: flex;
    justify-content: center;
    flex-direction: column;
    border-radius: 25px;
    margin-right: 10px;
}

p {
    padding-block-end: 21px;
    color: #b0a5bb;
    text-align: left;
    margin-left: 9px;
}

.prev,
.next {
    transform: translateY(-50%);
    padding: 10px;
}

.section-item {
    height: 200px;
    border-radius: 10px;
    flex: 0 0 auto;
    width: 255px;
    margin: 20px;
    display: flex;
    align-items: center;
    justify-content: left;
    flex-direction: column;
    padding: 25px;
    text-align: left;
    background-color: #f9f7fc;
    color: #965af9;
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;

}
</style>
  