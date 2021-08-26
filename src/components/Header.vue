<template>
  <header class="header">
    <!-- Logo -->
    <div class="logo">
      <img src="../assets/img/white-logo.png" alt="logo" class="logo-img" />
      <span class="name">Youshi</span>
    </div>
    <!-- Navigation bar -->
    <div class="navbar">
      <a href="" class="navbar-item">Home</a>
      <a href="" class="navbar-item">Product</a>
      <a href="" class="navbar-item">Promo</a>
      <a href="" class="navbar-item">About</a>
      <a href="" class="navbar-item">Contact</a>
    </div>
    <!-- Search button -->
    <div class="search">
      <img
        src="../assets/img/search-icon.png"
        alt="Search"
        class="search-icon"
      />
    </div>
    <!-- Mobile Menu -->
    <div class="menu">
      <img src="../assets/img/menu-mobile.png" alt="Menu" class="menu-icon" />
    </div>
  </header>
  <div class="navbar-mobile">
    <a href="" class="navbar-item">Home</a>
    <a href="" class="navbar-item">Product</a>
    <a href="" class="navbar-item">Promo</a>
    <a href="" class="navbar-item">About</a>
    <a href="" class="navbar-item">Contact</a>
  </div>
</template>
<script>
// export default {
//   data() {
//     return {
//       isOpen: false,
//     }
//   },
//   methods: {
//     openMenu(isOpen){
//       isOpen = !isOpen;
//       return isOpen;
//     }
//   }
// };
</script>
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
  .menu {
    display: none;
  }
  .navbar-mobile {
    display: none;
  }
}
// Responsive
@media only screen and (max-width: 600px) {
  .header {
    justify-content: space-between;
    .logo {
      padding-left: 20px;
      .logo-img {
        width: 40px;
        height: 40px;
      }
      .name {
        font-size: 16px;
      }
    }
    .navbar {
      display: none;
    }
    .search {
      display: none;
    }
    .menu {
      display: block;
      width: 70px;
      height: 50px;
      text-align: center;
      padding-top: 20px;
      .menu-icon {
        width: 30px;
        height: 30px;
      }
    }
  }
  .navbar-mobile {
    display: block;
    position: fixed;
    margin-top: 70px;
    width: 100%;
    height: 200px;
    background-color: $primary-blue;
    z-index: 5;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: center;
    .navbar-item {
      color: $text-color-white;
      font-size: 20px;
    }
  }
}
</style>
