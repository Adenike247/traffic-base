<template>
  <div class="items">
    <div>
      <div>
        <div class="check-item">
          <img class="check-icon" src="../assets/icon-check.svg" alt="check" />
          <p>Unlimited websites</p>
        </div>

        <div class="check-item">
          <img class="check-icon" src="../assets/icon-check.svg" alt="check" />
          <p>100% data ownwership</p>
        </div>
        <div class="check-item">
          <img class="check-icon" src="../assets/icon-check.svg" alt="check" />
          <p>Email reports</p>
        </div>
      </div>
    </div>
    <div class="btn-content">
      <button class="btn">Start my trial</button>
    </div>
  </div>
</template>
<script scoped></script>
<style scoped>
* {
  margin: 0;
  padding: 0;
  max-width: 1536px;
  margin: 0 auto;

  font-family: "inter";
}
.items {
  padding-left: 20px;
}
.check-item p {
  font-size: 1.4rem;
  color: hsl(225, 20%, 60%);
  padding-right: 4rem;
  text-align: center;
  align-items: center;
}
.btn-content{
    margin-right: 20px;

}

.btn {
  margin-top: 3rem;
  margin-bottom: 2rem;
  border: none;
  text-align: center;
  border-radius: 40px;
  padding: 26px 80px;
  background: hsl(227, 35%, 25%);
  color: hsl(223, 50%, 87%);
  font-size: 1.5rem;
}

.check-item {
  margin-left: 1rem;
  padding-bottom: 10px;
  display: flex;
  text-align: center;
  align-items: center;
}
.check-icon {
  width: 8px;
  height: 16px;
}
@media screen and (min-width: 768px) {
  * {
    margin: 0;
  }
  .items {
    display: flex;
    align-items: center;
  }
  .btn-content {
    margin-left: 50px;
  }
  .btn {
    padding: 14px 50px;
    font-size: 1.2rem;
  }
  .check-item {
    text-align: center;
    align-items: center;
  }
  .check-icon {
    width: 30px;
  }
}
</style>
