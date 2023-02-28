<template>
  <div>
    <div class="month_year">
      <p>Monthly Billing</p>
      <label class="switch">
        <input type="checkbox" />
        <span class="slider round"></span>
      </label>
      <p>Yearling Billing</p>
      <span>
        <p>-25% <span>discount</span></p>
      </span>
    </div>
    <div class="divider"></div>
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
.divider {
  margin-top: 3rem;
  margin-bottom: 2rem;
  width: 100%;
  background-color: hsl(224, 65%, 95%);
  border: 0.2px solid hsl(224, 65%, 95%);
}
.month_year {
  margin-top: 30px;
  padding-left: 15px;
  padding-right: 15px;
  display: flex;
  align-items: center;
  gap: 2px;
}
.month_year p {
  font-size: 0.9rem;
  color: hsl(225, 20%, 60%);
}
.month_year span p {
  font-weight: 400;
  color: hsl(15, 100%, 70%);
  background-color: hsl(14, 92%, 95%);
  padding: 8px 22px;
  border-radius: 12px;
  text-align: center;
}
.month_year span p span {
  display: none;
}

.switch {
  position: relative;
  display: inline-block;
  width: 48px;
  height: 26px;
}

.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: hsl(223, 50%, 87%);
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

.slider:before {
  position: absolute;
  content: "";
  height: 16px;
  width: 16px;
  left: 4px;
  bottom: 6px;
  background-color: hsl(0, 0%, 100%);
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

input:checked + .slider {
  background-color: hsl(223, 50%, 87%);
}
input:checked + .slider:before {
  -webkit-transform: translateX(26px);
  -ms-transform: translateX(26px);
  transform: translateX(26px);
}

/* Rounded sliders */
.slider.round {
  border-radius: 34px;
}

.slider.round:before {
  border-radius: 50%;
}
@media screen and (min-width: 768px) {
  .month_year span p span {
    display: inline;
  }
  .month_year {
    margin-left: 8rem;
    margin-right: 4rem;
  }
  .month_year {
    gap: 2px;
    padding-left: 2rem;
  }
}
</style>
