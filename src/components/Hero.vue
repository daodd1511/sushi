<template>
  <div class="hero">
    <div class="hero-content">
      <h1 class="title">Sushi</h1>
      <p class="description">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Et qui ea ad,
        architecto sit doloribus.
      </p>
      <button class="btn">ORDER NOW</button>
    </div>
  </div>
</template>

<script>
export default {};
</script>
<style lang="scss" scoped>
@import ".././assets/main.scss";
.hero {
  z-index: 3;
  padding-top: 70px;
  position: relative;
  background: url(../assets/img/Hero.jpg) center/cover no-repeat;
  .image {
    width: 100%;
  }
  .hero-content {
    color: #fff;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    align-content: flex-start;
    align-items: baseline;
    padding: 180px 0 70px 65px;
    gap: 40px;
    .title {
      font-size: 100px;
    }
    .description {
      font-size: 25px;
      max-width: 600px;
    }
  }
  .test {
    height: 100px;
  }
}
</style>
