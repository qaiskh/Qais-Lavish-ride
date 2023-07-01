<template>
    <div class="main-container3">

        <div class="image-section">
            <img class="image-section1" src="/public/pngegg.png" alt="" />
        </div>
        <div class="value-text-section">
            <div style="display: flex; align-items: center;">
                <div class="slider-icon2">
                    <v-icon style="font-size: 30px;" color="#ffe09e" icon="mdi-diamond-stone"></v-icon>
                </div>
                <div>
                    <h3>Our Value To Help You</h3>
                </div>
            </div>
            <div class="value-span-section">
                We Always want to provide the best value for you and your health , join us to maximize the benefits
            </div>
            <v-row align="center" no-gutters style="height: 150px; margin-inline: -2rem;">
                <div class="value-item">

                    <div class="slider-icon3 "><v-icon style="font-size: 30px; " color="#ffff"
                            icon="mdi-heart"></v-icon>
                    </div>

                    <div class="value-section">
                        <div class="value-card">

                            <h4 style=" margin-block-end: 15px;">Becomes healthier</h4>
                            <span> healthier recipes from food and nutriont expert </span>
                        </div>
                    </div>

                </div>
                <div class="value-item">
                    <div class="slider-icon3 "><v-icon style="font-size: 30px; " color="#ffe09e"
                            icon="mdi-trending-up"></v-icon>
                        </div>
                    <div class="value-section">
                        <div class="value-card">

                            <h4 style=" margin-block-end: 15px;"> Increase Energy</h4>
                            <span> healthier recipes from food and nutriont expert </span>
                        </div>
                    </div>

                </div>
                <div class="value-item">
                    <div class="slider-icon3 "><v-icon style="font-size: 30px; " color="#ffff"
                            icon="mdi-shield-check-outline"></v-icon>
                        </div>
                    <div class="value-section">

                        <div class="value-card">

                            <h4 style=" margin-block-end: 15px;"> Controlling Weight</h4>
                            <span> healthier recipes from food and nutriont expert </span>
                        </div>
                    </div>

                </div>
                <div class="value-item">
                    <div class="slider-icon3 "><v-icon style="font-size: 30px; " color="#ffff"
                            icon="mdi-star"></v-icon>
                        </div>
                    <div class="value-section">
                        <div class="value-card">

                            <h4 style=" margin-block-end: 15px;"> Becomes Happier</h4>
                            <span> healthier recipes from food and nutriont expert </span>
                        </div>
                    </div>

                </div>
            </v-row>
        </div>
    </div>
</template>
  
<script setup>
  //
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

.value-span-section {
    margin-block-start: 25px;
    padding-block-end: 25px;
    color: #a6a0b9;
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

.value-item {
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

.main-container3 {
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
</style>
  