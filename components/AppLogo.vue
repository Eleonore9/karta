<template>
  <div class="VueToNuxtLogo">
    <div class="Circle"/>
    <div class="Triangle Triangle--two"/>
    <div class="Triangle Triangle--one"/>
    <div class="Triangle Triangle--three"/>
    <div class="Triangle Triangle--four"/>
  </div>
</template>

<style>
.VueToNuxtLogo {
  display: inline-block;
  animation: turn 2s linear forwards 1s;
  transform: rotateX(180deg);
  position: relative;
  overflow: hidden;
  height: 180px;
  width: 245px;
  opacity: 0.9;
  z-index: 1;
}

.Circle {
  margin-left: 40px;
  margin-top: 14px;
  width: 150px;
  height: 150px;
  background: #526488;
  -moz-border-radius: 75px;
  -webkit-border-radius: 75px;
  border-radius: 75px;
}

.Triangle {
  position: absolute;
  top: 0;
  left: 0;
  width: 0;
  height: 0;
}

.Triangle--one {
  margin-left: 85px;
  margin-top: 0px;
  border-left: 30px solid transparent;
  border-right: 30px solid transparent;
  border-bottom: 60px solid #3b8070;
}

.Triangle--two {
  margin-top: 118px;
  margin-left: 85px;
  border-left: 30px solid transparent;
  border-right: 30px solid transparent;
  border-top: 60px solid #3b8070;
}

.Triangle--three {
  margin-top: 59px;
  margin-left: 25px;
  border-top: 30px solid transparent;
  border-right: 60px solid #3b8070;
  border-bottom: 30px solid transparent;
}

.Triangle--four {
  margin-top: 59px;
  margin-left: 145px;
  border-left: 60px solid #3b8070;
  border-top: 30px solid transparent;
  border-bottom: 30px solid transparent;
}

@keyframes turn {
  100% {
    transform: rotateX(0deg);
  }
}

@keyframes godown {
  100% {
    top: 180px;
  }
}

@keyframes goright {
  100% {
    left: 70px;
  }
}
</style>
