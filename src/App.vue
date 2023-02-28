<template>
  <div class="main-container">
    <div class="content">
      <div class="header">
        <img
          class="background-img"
          src="./assets/pattern-circles.svg"
          alt="background-img"
        />

        <h2>{{ title }}</h2>
        <p>
          Sign-up for our 30-day trial. <br />
          No credit card required.
        </p>
        <h3 class="subtopic">
          Sign-up for our 30-day trial. No credit card required.
        </h3>
      </div>
    </div>
    <simplecard></simplecard>
  </div>
</template>

<script>
import SimpleCard from "./components/SimpleCard.vue";
export default {
  components: {
    simplecard: SimpleCard,
  },
  data() {
    return {
      title: "Simple, traffic-based pricing",
    };
  },
};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  max-width: 1536px;
  margin: 0 auto;
  font-family: "inter";
}
.header {
  padding-top: 3rem;
}
.main-container {
  text-align: center;
  background: url(./assets/bg-pattern.svg) no-repeat;
  justify-content: center;
  align-items: center;
}
.subtopic {
  display: none;
}

.main-container h2 {
  padding-top: 2rem;
  font-size: 1.8rem;
  color: hsl(227, 35%, 25%);
  padding-bottom: 20px;
}
.main-container p {
  font-size: 1.2rem;
  color: hsl(225, 20%, 60%);
}
.background-img {
  position: absolute;
  margin-top: 10px;
  left: 120px;
  height: 200px;
}
@media screen and (min-width: 768px) {
  .background-img {
    left: 40%;
  }
  .main-container h2 {
    font-size: 3rem;
  }
  .main-container p {
    display: none;
  }
  .subtopic {
    display: block;
    font-size: 1.4rem;
    color: hsl(225, 20%, 60%);
  }
}
</style>
