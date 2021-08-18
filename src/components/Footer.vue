<template>
  <footer class="footer">
    <div class="social-media">
      <h3>Title Here</h3>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ipsa magni sed aliquam quibusdam perferendis non nobis corrupti impedit voluptates tenetur!</p>
      <div class="social-icons">
        <div class="icon">
          <img src="@/assets/img/instagram.png" alt="instagram" class="instagram">
        </div>
        <div class="icon">
          <img src="@/assets/img/facebook.png" alt="facebook" class="facebook">
        </div>
        <div class="icon">
          <img src="@/assets/img/twitter.png" alt="twitter" class="twitter">
        </div>
        <div class="icon">
          <img src="@/assets/img/whatsapp.png" alt="whatsapp" class="whatsapp">
        </div>
      </div>
    </div>
    <div class="contact">
      <div class="about">
        <h3>About</h3>
        <a href="#">History</a><br><br>
        <a href="#">Our Team</a><br><br>
        <a href="#">Brand Guidelines</a><br><br>
        <a href="#">Terms & Conditions</a><br><br>
        <a href="#">Privacy Policy</a>
      </div>
      <div class="services">
        <h3>Services</h3>
        <a href="#">How to Orders</a><br><br>
        <a href="#">Our Product</a><br><br>
        <a href="#">Order Status</a><br><br>
        <a href="#">Promo</a><br><br>
        <a href="#">Payment Method</a>
      </div>
      <div class="others">
        <h3>Others</h3>
        <a href="#">Contact Us</a><br><br>
        <a href="#">Help</a><br><br>
        <a href="#">Privacy</a>
      </div>
    </div>
  </footer>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>
@import "@/assets/main.scss";
.footer {
  height: 350px;
  background-color: black;
  color:$text-color-white;
  display: flex;
  justify-content:space-evenly;
  gap: 0 20px;
  padding: 200px 0 200px 0;
  h3{
    font-size: 30px;
    padding-bottom: 40px;
    font-weight: normal;
  }
  .social-media{
    max-width: 30%;
    max-height: 70%;
    p{
      font-size: 23px;
      padding-bottom: 40px;
    }
    .social-icons{
      display: flex;
      gap: 20px;
      .icon{
        @include rounded(45px,$radius: 50%);
        background-color: white;
        position: relative;
        .instagram,.facebook,.twitter,.whatsapp{
          position: absolute;
          height: 60%;
          top: 20%;
          left: 20%;
        }
      }
    }
  }
  .contact{
    display: flex;
    gap: 40px;
    max-height: 70%;
    a{
      color: white;
      font-size: 23px;
      padding-bottom: 10px;
    }
  }
}
</style>