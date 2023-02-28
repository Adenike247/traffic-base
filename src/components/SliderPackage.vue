<template>
  <div class="slider">
    <h1></h1>
    <div class="slider-icon">
      <img src="../assets/icon-slider.svg" alt="slider" />
    </div>
    <p></p>
  </div>
</template>
<script></script>
<style scoped>
* {
  margin: 0;
  padding: 0;
  max-width: 1536px;
  margin: 0 auto;
  font-family: 'inter';

}

.slider {
  display: flex;
  align-items: center;
  padding-left: 15px;
  padding-right: 10px;
}
.slider-icon {
  align-items: center;
  padding: 24px 20px;
  border-radius: 50%;
  text-align: center;
  background-color: hsl(174, 86%, 45%);
  box-shadow: 5px 10px 22px hsl(174, 86%, 45%);
}
h1,
p {
  height: 14px;
  width: 164px;
  border-radius: 20px;
  background: hsl(174, 77%, 80%);
}
p {
  background-color: hsl(224, 65%, 95%);
}
@media screen and (min-width: 768px) {
  .slider {
    padding-left: 60px;
    padding-right: 60px;
  }
  h1,
  p {
    width: 18rem;
  }

}
</style>
