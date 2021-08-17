<template>
  <section class="statistic">
    <h1 class="title">Statistics</h1>
    <p class="description">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Itaque blanditiis dicta, deleniti ut iure quos?</p>
    <div class="statistic-details">
      <div class="detail">
        <h1>123</h1>
        <p>STORE</p>
      </div>
      <div class="detail">
        <h1>100</h1>
        <p>MENU</p>
      </div>
      <div class="detail">
        <h1>200</h1>
        <p>CHEF</p>
      </div>
    </div>
    <!-- Decorator -->
    <img src="@/assets/img/yellowdot.svg" alt="dot" class="dot1">
    <img src="@/assets/img/yellowdot.svg" alt="dot" class="dot2">
    <img src="@/assets/img/yellowround.svg" alt="round" class="round1">
    <img src="@/assets/img/yellowround.svg" alt="round" class="round2">
    <img src="@/assets/img/yellowwavy.svg" alt="wavy" class="wavy1">
    <img src="@/assets/img/yellowwavy.svg" alt="wavy" class="wavy2">
  </section>
</template>
<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>
@import "@/assets/main.scss";
.statistic{
  height:750px;
  text-align:center;
  background-color: $primary-blue;
  color: $text-color-white;
  overflow: hidden;
  position: relative;
  .title{
    font-size: 55px;
    padding-top: 80px;
  }
  .description{
    max-width: 650px;
    margin: auto;
    font-size: 23px;
    padding: 35px 0 80px 0;
  }
  .statistic-details{
    display:  flex;
    justify-content: space-evenly;
    .detail{
      @include rounded(270px,$radius:50%);
      border: 5px solid $text-color-white;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      h1{
        font-size: 80px;
      }
      p{
        font-size: 40px;
        font-weight: bold;
      }
    }
  }
  // Decorator
  .dot1{
    position: absolute;
    top: 50px;
    left: 50px;
  }
  .dot2{
    position: absolute;
    bottom: 40px;
    padding-left: 120px;
  }
  .round1{
    position: absolute;
    bottom: -70px;
    left: 300px;
  }
  .round2{
    position: absolute;
    top: 80px;
    right: 30px;
  }
  .wavy1{
    position: absolute;
    bottom: 85px;
    right: 15px;
  }
  .wavy2{
    position: absolute;
    top: 220px;
    left: 60px;
  }
}
</style>