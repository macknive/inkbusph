<template>
  <div class="main">
    <div class="welcome">
      <div class="welcome-text">
        <div class="bus-image">
          <img src="../assets/bbss.png" alt="" class="bus" />
        </div>
        <div class="container">
          <div class="title-container">
            <img src="../assets/ib.png" alt="" class="title" />
          </div>
          <div class="subtitle">
            <h2>Professional Ink Mastery Beyond the Surface</h2>
          </div>

          <div class="socials">
            <p>Follow us on our official social accounts</p>
            <div class="social">
              <a href="https://www.facebook.com/InkBusPh">
                <img src="../assets/facebook.png" height="30"
              /></a>
              <a href="https://www.tiktok.com/@inkbusph"
                ><img src="../assets/tiktok.png" height="30"
              /></a>
              <a
                href="https://www.youtube.com/channel/UC2eu3_qCMICON-Llv9gZGtA"
              >
                <img src="../assets/youtube.png" height="30"
              /></a>
              <a href="https://www.instagram.com/inkbus.ph/?hl=en"
                ><img src="../assets/instagram.png" height="30"
              /></a>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="ink-container">
      <div class="inks">
        <div class="ink-text">
          <h1>Our Inks</h1>

          <p>Made for tattoo artists by tattoo artists</p>
          <p>
            It's time to set a new standard. In our industry's long history, a
            lot has changed. Machines have more powerful motors than ever
            before. Stencils can be printed to photographic quality. Cartridge
            needles took the industry by storm. Ink caps are even advancing.
          </p>
          <p>
            So much time, money and energy are spent on the products we use, yet
            the inks have remained the same. The ink industry hasn’t deviated
            from the original formula. Empire has raised the standard and
            brought the fundamentals of art into the industry. Combining
            knowledge of art and tattooing with the best chemists in the field,
            we bring you a safe and consistent ink to work with.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script></script>

<style lang="scss" scoped>
h1 {
  text-align: center;
}
.welcome {
  background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.5)),
    url("../assets/bg.jpg");
  background-size: cover;
  background-position: center;
  width: 100%;
  min-height: 800px; /* Set a minimum height */
  height: 100%;
  display: flex; /* Make .welcome a flex container */
  flex-direction: column;
  justify-content: center; /* Center children horizontally */
  align-items: center;

  .welcome-text {
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    justify-content: center; /* Center children horizontally */
    align-items: center;
  }

  .social {
    display: flex;
    flex-direction: row;
    a {
      margin-right: 12px;
    }
  }
}
.ink-container {
  height: auto;
  width: 100%;
  .inks {
    background-image: url("../assets/inks.png");
    min-height: 400px;
    background-size: cover;
    background-position: center;
    padding: 50px 30px;
  }
  .ink-text {
    width: 50%;
  }
}

.work-samples {
  padding: 20px;
  h1 {
    margin: 0;
  }
  background-color: white;
  color: black;
  min-height: 500px;
}

.title-container {
  display: flex;
  flex-direction: "column";
}

.socials {
  display: flex;
  flex-direction: column;
}

.subtitle {
  margin-bottom: 0;
}

@media screen and (max-width: 450px) {
  .title-container {
    .title {
      height: 80px;
      margin: auto;
    }
  }
  .socials {
    align-items: center;
    margin-bottom: 20%;
  }
  .subtitle {
    text-align: center;
    padding: 0 30px;
    font-size: 16px;
  }
  .ink-text {
    width: 100% !important;
  }
  .bus-image {
    margin-top: 20%;
  }
  .bus {
    height: 400px;
  }
}
</style>
