<script setup>
import { RouterLink, RouterView } from "vue-router"
</script>

<template>
  <!-- <header>
    <div class="wrapper">
      <nav>
        <RouterLink to="/">home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header> -->

  <div class="container">
    <h3>Cris Palacio's</h3>
    <img class="logo" src="../src/assets/inkbus.png" alt="" height="" />
    <h2>Website opening soon</h2>
    <h2>Follow us on our official social accounts</h2>
    <div class="social">
      <a href="https://www.facebook.com/InkBusPh">
        <img src="../src/assets/facebook.png" height="50"
      /></a>
      <a href="https://www.tiktok.com/@inkbusph"
        ><img src="../src/assets/tiktok.png" height="50"
      /></a>
      <a href="https://www.youtube.com/channel/UC2eu3_qCMICON-Llv9gZGtA">
        <img src="../src/assets/youtube.png" height="50"
      /></a>
      <a
        href="https://www.instagram.com/explore/locations/107680801880021/ink-bus-ph/"
        ><img src="../src/assets/instagram.png" height="50"
      /></a>
    </div>
  </div>

  <RouterView />
</template>

<style scoped>
p {
  text-align: left;
  align-items: left;
  margin: 0;
}
.container {
  margin-top: 100px;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.logo {
  height: auto;
  width: 100%;
  object-fit: contain;
}
a {
  color: white;
}
.social {
  margin: 60px 0 20px;
  display: flex;
  flex-direction: row;
}
.social img {
  padding: 12px;
}
h2 {
  text-align: center;
}
</style>
