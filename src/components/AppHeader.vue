<script>
export default {
  name: 'AppHeader',

  data() {
    return {
      links: [
        {
          name: "Home",
          hover: false
        },
        {
          name: "Games",
          hover: true
        },
        {
          name: "Shop",
          hover: true
        },
        {
          name: "Pages",
          hover: true
        },
        {
          name: "Blog",
          hover: true
        },
        {
          name: "Contact",
          hover: false
        },
      ]
    }
  }
}
</script>

<template>

  <header>
    <div class="container">

      <nav>
        <div class="menu">

          <div class="left_menu">
            <img src="../assets/images/logo.png" alt="">
          </div>
          <!-- /.left_menu -->

          <div class="mid_menu">
            <ul class="links" v-for="link in links">
              <li class="link_name">{{ link.name }} <i v-if="link.hover" class="fa-solid fa-angle-down"></i> </li>
            </ul>
          </div>
          <!-- /.mid_menu -->

          <div class="right_menu">
            <img class="cart_icon" src="../assets/images/icon/cart-icon.png" alt="">
            <button class="btn">LIVE STREAMING</button>
          </div>
          <!-- /.right_menu -->

        </div>
        <!-- /.menu -->
      </nav>
      <!-- /.nav -->

      <div class="index-banner">
        <div class="row">

          <div class="col-5">

            <div class="card">
              <div class="sub-title">Game With Live Streaming</div>
              <div class="card-title">Future Of Esports</div>
              <div class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Perspiciatis, iste quod? Voluptatum quos voluptate nam facere atque tempora illo
                consequatur!</div>
              <div class="card-btn">
                <button class="btn">Explore Games</button>
                <img class="play-icon" src="../assets/images/icon/play-icon.png" alt="">
              </div>

            </div>

          </div>

          <div class="col-7">
            <img class="img banner-image" src="../assets/images/index-banner-illus.png" alt="">
          </div>

        </div>

      </div>
      <!-- /.index-banner -->


    </div>
  </header>
  <!-- /header -->


</template>

<style>

</style>
