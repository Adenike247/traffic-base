<template>
  <section class="card">
    <div class="card-section">
      <div class="page-view">
        <h3>100K PAGEVIEWS</h3>
        <h3 class="money-notdisplay"><span>$16.00 </span>/month</h3>
      </div>
      <sliderpackage></sliderpackage>
      <h3 class="money-month"><span>$16.00</span> / month</h3>
      <monthyear></monthyear>
      <div></div>
      <itemselect></itemselect>
    </div>
  </section>
</template>
<script>
import MonthYear from "./MonthYear.vue";
import SliderPackage from "./SliderPackage.vue";
import ItemSelect from "./ItemSelect.vue";

export default {
  components: {
    monthyear: MonthYear,
    sliderpackage: SliderPackage,
    itemselect: ItemSelect,
  },
};
</script>
<style scoped>
* {
  margin: 0;
  padding: 0;
  max-width: 1536px;
  margin: 0 auto;
  font-family: 'inter';
}
.card {
  align-items: center;
}
.card-section {
  text-align: center;
  margin-top: 8.2rem;
  background: hsl(0, 0%, 100%);
  border-radius: 10px;
  box-shadow: 5px 10px 18px #888888;
}
.page-view{
  margin-left: 30px;
}
.page-view h3 {
  padding-top: 4rem;
  padding-bottom: 1rem;
  text-align: center;
  font-size: 1.5rem;
  color: hsl(225, 20%, 60%);
  letter-spacing: 2px;
}
.money-notdisplay{
  display: none;
}
.money-month {
  margin-top: 2rem;
  text-align: center;
  align-items: center;
  padding-right: 4rem;
  font-size: 1.5rem;
  display: flex;
  color: hsl(225, 20%, 60%);
}

.money-month span {
  padding-left: 2.2rem;
  font-size: 2.3rem;
  color: hsl(227, 35%, 25%);
}
@media screen and (min-width: 768px) {
  .card {
    width: 700px;
  }
  .page-view h3 {
    margin-bottom: 30px;
  }
  

.money-notdisplay {
  text-align: center;
  align-items: center;
  padding-right: 3rem;
  font-size: 2rem;
  gap: 6px;
  display: flex;
  color: hsl(225, 20%, 60%);
}

.money-notdisplay span{
  padding-left: 2rem;
  font-size: 3rem;
  color: hsl(227, 35%, 25%);
}
.money-month{
  display: none;
}
.page-view{
    display: flex;
    align-items: center;
  }
}
</style>
