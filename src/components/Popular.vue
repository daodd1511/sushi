<template>
  <section class="popular">
    <div class="popular-heading">
      <h1>Popular Menu</h1>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.  Quisquam pariatur eaque molestias rerum, iusto at.</p>
    </div>
    <div class="popular-items">
      <div class="popular-item">
        <img src="../assets/img/sushi1-copy.jpg" alt="sushi1" class="sushi-img">
        <h2>Title</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing</p>
      </div>
      <div class="popular-item">
        <img src="../assets/img/sushi2-copy.jpg" alt="sushi2" class="sushi-img">
        <h2>Title</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing</p>
      </div>
      <div class="popular-item">
        <img src="../assets/img/sushi3-copy.jpg" alt="sushi3" class="sushi-img">
        <h2>Title</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing</p>
      </div>
    </div>
    <img src="../assets/img/yellowdot.svg" alt="dot" class="dot1">
    <img src="../assets/img/yellowdot2.svg" alt="dot" class="dot2">
    <img src="../assets/img/yellowround.svg" alt="round" class="round1">
    <img src="../assets/img/yellowround.svg" alt="round" class="round2">
    <img src="../assets/img/yellowwavy.svg" alt="wavy" class="wavy1">
    <img src="../assets/img/yellowwavy.svg" alt="wavy" class="wavy2">
  </section>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>
@import "@/assets/main.scss";
.popular{
  z-index: 2;
  position:relative;
  height: 750px;
  background-color: $primary-blue;
  color: $text-color-white;
  text-align: center;
  .popular-heading{
    padding-bottom: 60px;
    h1{
      font-size:55px;
      padding-top: 80px;
      padding-bottom: 35px;
    }
    p{
      font-size:23px;
      max-width: 700px;
      margin: auto;
    }
  }
  .popular-items{
    display: flex;
    justify-content: space-evenly;
    .popular-item{
      .sushi-img{
        @include rounded(240px,$radius:50%);
      }
      h2{
        padding: 15px 0 20px 0;
      }
      p{
        max-width: 250px;
      }
    }
  }
  .dot1{
    position: absolute;
    top: -12px;
    left: 170px;
    width: 150px;
  }
  .dot2{
    position: absolute;
    height: 150px;
    right: -12px;
    bottom: 250px;
  }
  .round1{
    position: absolute;
    width: 150px;
    top: -25px;
    right: -30px;
  }
  .round2{
    position: absolute;
    width: 150px;
    left: -70px;
    bottom: 100px;
  }
  .wavy1{
    position: absolute;
    width: 80px;
    right: 0;
    bottom: 60px;
  }
  .wavy2{
    position: absolute;
    width: 80px;
    left: 60px;
    top: 150px;
  }

}

</style>