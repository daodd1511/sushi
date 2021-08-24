<template>
  <header class="header">
    <section class="logo">
      <img src="../assets/img/white-logo.png" alt="logo" class="logo-img" />
      <span class="name">Youshi</span>
    </section>
    <section class="navbar">
      <a href="" class="navbar-item">Home</a>
      <a href="" class="navbar-item">Product</a>
      <a href="" class="navbar-item">Promo</a>
      <a href="" class="navbar-item">About</a>
      <a href="" class="navbar-item">Contact</a>
    </section>
    <section class="search">
      <img
        src="../assets/img/search-icon.png"
        alt="Search"
        class="search-icon"
      />
    </section>
  </header>
</template>
<script></script>
<style lang="scss" scoped>
@import ".././assets/main.scss";
.header {
  z-index: 10;
  height: 70px;
  width: 100%;
  background-color: $primary-blue;
  display: flex;
  justify-content: space-around;
  align-items: center;
  position: fixed;
  user-select: none;
  .logo {
    display: flex;
    align-items: center;
    cursor: pointer;
    .logo-img {
      width: 50px;
      height: 50px;
      color: white;
      padding-right: 3px;
    }
    .name {
      color: $text-color-white;
      font-weight: bold;
      font-size: 20px;
      text-align: center;
    }
  }
  .navbar {
    display: flex;
    gap: 0 45px;
    .navbar-item {
      color: $text-color-white;
      font-size: 20px;
    }
  }
  .search {
    .search-icon {
      width: 25px;
      height: 25px;
      padding-top: 10px;
      cursor: pointer;
    }
  }
}
</style>
