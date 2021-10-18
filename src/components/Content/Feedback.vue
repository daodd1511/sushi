<template>
  <section class="feedback">
    <div class="background-layer">
      <div class="content">
        <img
          src="https://i.ibb.co/QjBp8DS/person2.jpg"
          alt="person"
          class="person-img"
        />
        <p>
          If you are a culinary fan, if you like to spend time in your kitchen,
          you likely find yourself looking for reliable resources through which
          you can
        </p>
        <h3>Phoebe Frazier</h3>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../../assets/main.scss";
.feedback {
  height: 750px;
  background: url("https://i.ibb.co/gDvn7cY/sushi3.jpg") center/cover no-repeat;
  color: $text-color-white;
  .background-layer {
    width: 100%;
    height: 100%;
    background-color: rgba(23, 17, 78, 0.8);
    .content {
      text-align: center;
      padding-top: 115px;
      .person-img {
        @include rounded(250px, $radius: 50%);
      }
      p {
        font-size: 40px;
        max-width: 75%;
        margin: 0 auto;
        padding: 35px 0 45px 0;
      }
      h3 {
        font-size: 45px;
      }
    }
  }
}
</style>
