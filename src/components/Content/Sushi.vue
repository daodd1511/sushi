<section class="sushi-container">
<img src="@/assets/img/sushi1-copy.jpg" alt="sushi1" class="sushi-img" />
<div class="sushi-content">
  <h1 class="title">Title Here</h1>
  <p class="description">
    Lorem ipsum, dolor sit amet consectetur adipisicing elit. Necessitatibus
    sequi tenetur eaque quod consequuntur optio.
  </p>
  <button class="btn">ORDER NOW</button>
</div>
<!-- Decorator -->
<img src="@/assets/img/round.svg" alt="round" class="round1" />
<img src="@/assets/img/round.svg" alt="round" class="round2" />
<img src="@/assets/img/dot.svg" alt="dot" class="dot1" />
<img src="@/assets/img/verticaldot.svg" alt="dott" class="dot2" />
<img src="@/assets/img/wavy.svg" alt="wavy" class="wavy" />
</section>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../../assets/main.scss";
.sushi-container {
  position: relative;
  background-color: $primary-yellow;
  height: 750px;
  display: flex;
  align-items: center;
  justify-content: space-around;
  overflow: hidden;
  .sushi-img {
    @include rounded(450px, $radius: 50%);
    margin-left: 100px;
    z-index: 3;
  }
  .sushi-content {
    color: $primary-blue;
    .title {
      font-size: 70px;
    }
    .description {
      max-width: 550px;
      font-size: 24px;
      padding: 30px 0 60px 0;
    }
  }
  //Decorator
  .round1 {
    position: absolute;
    right: -40px;
    bottom: 65px;
  }
  .round2 {
    z-index: 2;
    position: absolute;
    top: 120px;
    left: 140px;
  }
  .dot1 {
    position: absolute;
    top: 30px;
    right: 20px;
  }
  .dot2 {
    position: absolute;
    bottom: 60px;
    left: 40px;
  }
  .wavy {
    position: absolute;
    top: 60px;
    padding-left: 230px;
  }
}
</style>
