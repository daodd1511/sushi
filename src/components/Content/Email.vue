<template>
  <section class="email">
    <h1>Title Here</h1>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Excepturi iure corporis, dolore obcaecati explicabo adipisci.</p>
    <div class="input-section">
      <div class="email-input">
        <input 
          type="text" 
          class="input email-detail" 
          placeholder="Your Email"
        >
      </div>
      <button class="btn">SUBCRIBE</button>
    </div>
    <!-- Decorator -->
    <img src="@/assets/img/dot.svg" alt="dot" class="dot1">
    <img src="@/assets/img/dot2.svg" alt="dot" class="dot2">
    <img src="@/assets/img/round.svg" alt="round" class="round1">
    <img src="@/assets/img/round.svg" alt="round" class="round2">
    <img src="@/assets/img/wavy.svg" alt="wavy" class="wavy1">
    <img src="@/assets/img/wavy.svg" alt="wavy" class="wavy2">

  </section>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>
@import "@/assets/main.scss";
.email{
  height: 600px;
  background-color: $primary-yellow;
  position: relative;
  text-align: center;
  color: $primary-blue;
  padding-top: 150px;
  h1{
    font-size: 70px;
  }
  p{
    max-width: 60%;
    margin: 0 auto;
    font-size: 25px;
    padding: 50px 0 80px 0;
  }
  .input-section{
    width: 60%;
    display: flex;
    justify-content: center;
    position: relative;
    margin: 0 auto;
    .email-input{
      width: 85%;
      background-color: white;
      height: 65px;
      border-radius: 60px;
      position: relative;
      .email-detail{
        outline: none;
        border: none;
        height: 100%;
        width: 60%;
        position: absolute;
        left: 30px;
        font-size: 24px;
      }
    }
    .btn{
      position: absolute;
      right: 5%;
      width: 230px;
    }
  }
  // Decorator
  .dot1{
    position: absolute;
    bottom: 70px;
    right: 100px;
  }
  .dot2{
    position: absolute;
    top: 80px;
    left: 90px;
  }
  .round1{
    position: absolute;
    bottom: 40px;
    width: 150px;
  }
  .round2{
    position: absolute;
    width: 150px;
    top: 10px;
    right: -40px;
  }
  .wavy1{
    position: absolute;
    left: 80px;
    bottom: 130px;
  }
  .wavy2{
    position: absolute;
    top: 60px;
    right: 240px;
  }
}
</style>