<template>
  <div style="padding: 5rem;">
    <div style="display: flex; justify-content: space-between; margin-inline: 2rem;">
      <div style="display: flex; align-items: center;">
        <div class="slider-icon2">
              <v-icon
              style="font-size: 30px;"
               color="#ffe09e"
              icon="mdi-crown"
             ></v-icon>
            </div>
      <div>
        <h3>Our Best Programs</h3>
      </div>
      </div>
      <div style="display: flex; justify-content: flex-end;">
        <div class="icon-container2">
          <v-icon
            style="font-size: 30px;"
            id="carousel-prev"
            color="grey"
            icon="mdi-chevron-left"
           ></v-icon>
        </div>
        <div class="icon-container2">
          <v-icon
            style="font-size: 30px;"
            id="carousel-next"
            color="grey"
            icon="mdi-chevron-right"
           ></v-icon>
        </div>

      </div>

    </div>

    <div class="main-container2">
      <div class="carousel-container">
        <div class="carousel-items">
          <!-- Place your carousel items here -->
          <div v-for="(item, index) in 10"  :key="index" class="carousel-item">
            <div class="slider-icon">
              <v-icon
              style="font-size: 30px;"
               color="#ffe09e"
              icon="mdi-chef-hat"
             ></v-icon>
            </div>
            <h4 style=" margin-block-end: 15px;"> Healthy Recipe</h4>
            <span> healthier recipes from food and nutriont expert </span>
          </div>
          <!-- <div class="carousel-item">Item 2</div>
        <div class="carousel-item">Item 3</div>
        <div class="carousel-item">Item 3</div>
        <div class="carousel-item">Item 3</div>
        <div class="carousel-item">Item 3</div>
        <div class="carousel-item">Item 3</div>
        <div class="carousel-item">Item 3</div>
        <div class="carousel-item">Item 3</div>
        <div class="carousel-item">Item 3</div>
        <div class="carousel-item">Item 3</div>
        <div class="carousel-item">Item 3</div>
        <div class="carousel-item">Item 3</div>
        <div class="carousel-item">Item 3</div> -->
          <!-- Add more carousel items as needed -->
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
  container = document.querySelector('.carousel-container')
  itemsContainer = document.querySelector('.carousel-items')
  items = document.querySelectorAll('.carousel-item')

  itemWidth = items[0].offsetWidth

  // Set the width of items container based on the number of items
  itemsContainer.style.width = `${itemWidth * items.length}px`

  // Add event listeners for arrow navigation
  const prevButton = document.getElementById('carousel-prev')
  const nextButton = document.getElementById('carousel-next')

  if (prevButton && nextButton) {
    prevButton.addEventListener('click', scrollCarousel.bind(null, 'prev'))
    nextButton.addEventListener('click', scrollCarousel.bind(null, 'next'))
  } else {
    console.error('Previous or Next button element not found.')
  }
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
.icon-container2 {

  cursor: pointer;
  margin-inline: 10px;
  background-color: rgb(255, 255, 255);
  padding: 10px;
  border-radius: 50%;
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}
.main-container2 {
  padding: 15px;
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
  margin: 7rem 2rem;
  border-radius: 20px;

}

.carousel-container {
  height: 200px;
  position: relative;
  overflow: hidden;
  border-radius: 20px;
  color: white;

}
/* .carousel-container:hover{
    height: 200px;

  position: relative;
  overflow: visible;
  border-radius: 20px;
  color: white;
width: 300px;
} */

.carousel-items {

  border-radius: 20px;
  transition: transform 0.5s ease-in-out;
  display: flex;
}


.carousel-item {
  height: 200px;

  flex: 0 0 auto;
  width: 300px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding: 40px;
  text-align: center;
  background-color: #965af9;
  transition: transform 0.1s ease-in-out, height 0.1s ease-in-out;


}

.carousel-item:hover {
  flex: 0 0 auto;
  width: 300px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding: 40px;
  text-align: center;
  background-color: #ffd66d;
  border-radius: 20px;
  transform: scale(1.1);

color: black;

.slider-icon{
  background-color: #edae30;
  border: 1px solid white;
}

}

.slider-icon{
  border: 1px solid gold;
  border-radius: 10px;
  padding: 10px;
  background-color: blueviolet;
  margin-block-end: 15px;
}

.slider-icon2{
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
   border-radius: 10px;
  padding: 10px;
  background-color: #965af9;
  margin-inline-end: 15px;
}
</style>