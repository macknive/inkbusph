<template>
  <nav class="dflex row">
    <a @click="scrollToTop" class="logo">
      <img src="../assets/inkbus.png" alt=""
    /></a>
    <a a @click="scrollToTop">Home</a>
    <a @click="scrollToGallery">Gallery</a>
    <a @click="scrollToAppointment">Appointment</a>
  </nav>
</template>

<script setup>
const scrollToGallery = () => {
  const gallery = document.querySelector(".swipes")
  gallery.scrollIntoView({ behavior: "smooth" })
}

const scrollToTop = () => {
  window.scrollTo({ top: 0, behavior: "smooth" })
}

const scrollToAppointment = () => {
  const appointment = document.querySelector(".appointment")
  appointment.scrollIntoView({ behavior: "smooth" })
}
</script>

<style lang="scss" scoped>
a {
  cursor: pointer;
}
img {
  height: 50px;
}
nav {
  padding-left: 20px;
  justify-content: start;
  width: 100%;
  height: 80px;
  a {
    margin-right: 12px;
  }
  .logo {
    height: auto;
  }
  @media screen and (max-width: 450px) {
    position: fixed;
    background: black;
    z-index: 10;
    a {
      margin-right: 4px;
    }
  }
}
</style>
