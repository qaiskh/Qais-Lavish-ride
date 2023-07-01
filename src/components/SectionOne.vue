<template>
  <div class="main-container">
    <div class="text-section">
      <div class="color-text">
        changing your
        <div class="dropping-texts">
          <div>eating</div>
          <div>lifestyle</div>
          <div>sleeping</div>
        </div>
        habits
      </div>
      <div class="span-section">
        Always take care of your health ss starting from the food menu that you
        consume every day
      </div>
      <div class="button-section">
        <button class="first-btn">Explore Menu</button>
        <div class="video-section">
          <div class="icon-container">
            <v-icon style="font-size: 50px;" color="warning" icon="mdi-play" size="x-large"></v-icon>
          </div>
          <div class="text-size">Watch Video</div>
        </div>
      </div>
    </div>
    <div class="image-section">
      <img class="image-section1" src="/public/pngegg.png" alt="" />
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
.button-section {
  justify-content: space-between;
  display: flex;
  margin-block-start: 35px;
}

.span-section {
  margin-block-start: 25px;
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
.main-container {
  display: flex;
  justify-content: space-between;
  padding: 5rem 5rem;
  height: 85vh;
  animation: bg 5s linear infinite;
  background-color: #8d4aeb;
}

.text-section {
  width: 600px;
  margin: 0px;
  color: #fff;
  font-family: 'Roboto';
}

.image-section {
}

.dropping-texts {
  display: inline-block;
  width: 130px;
  text-align: left;
  height: 90px;
  vertical-align: -2px;
  color: gold;
}

.dropping-texts > div {
  font-size: 0px;
  opacity: 0;
  margin-left: -30px;
  position: absolute;
  font-weight: 700;
}

.dropping-texts > div:nth-child(1) {
  animation: roll 5s linear infinite 0s;
}
.dropping-texts > div:nth-child(2) {
  animation: roll 5s linear infinite 1s;
}
.dropping-texts > div:nth-child(3) {
  animation: roll2 5s linear infinite 3s;
}
/* .dropping-texts > div:nth-child(4) {
  animation: roll2 5s linear infinite 3s;
} */

@keyframes roll {
  0% {
    font-size: 0px;
    opacity: 0;
    margin-left: -30px;
    margin-top: 0px;
    transform: rotate(-25deg);
  }
  3% {
    opacity: 1;
    transform: rotate(0deg);
  }
  5% {
    font-size: inherit;
    opacity: 1;
    margin-left: 0px;
    margin-top: 0px;
  }
  20% {
    font-size: inherit;
    opacity: 1;
    margin-left: 0px;
    margin-top: 0px;
    transform: rotate(0deg);
  }
  27% {
    font-size: 0px;
    opacity: 0.5;
    margin-left: 20px;
    margin-top: 100px;
  }
  100% {
    font-size: 0px;
    opacity: 0;
    margin-left: -30px;
    margin-top: 0px;
    transform: rotate(15deg);
  }
}

@keyframes roll2 {
  0% {
    font-size: 0px;
    opacity: 0;
    margin-left: -30px;
    margin-top: 0px;
    transform: rotate(-25deg);
  }
  3% {
    opacity: 1;
    transform: rotate(0deg);
  }
  5% {
    font-size: inherit;
    opacity: 1;
    margin-left: 0px;
    margin-top: 0px;
  }
  30% {
    font-size: inherit;
    opacity: 1;
    margin-left: 0px;
    margin-top: 0px;
    transform: rotate(0deg);
  }
  37% {
    font-size: 1500px;
    opacity: 0;
    margin-left: -1000px;
    margin-top: -800px;
  }
  100% {
    font-size: 0px;
    opacity: 0;
    margin-left: -30px;
    margin-top: 0px;
    transform: rotate(15deg);
  }
}

@keyframes bg {
  25% {background: #8947f2;}
  50% {background: #8744f3;}
  0% {background: #ae7cfe;}
  100% {background: #854fdc;}
   75% {background: #a051d3;}
}
</style>
