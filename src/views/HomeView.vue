<template>
  <div class="home-view">
    <div class="top-bar">
      <div class="logo">JPM</div>
      <div class="spacer"></div>
      <div class="menu">
        <menu-bar></menu-bar>
      </div>
    </div>
    <div class="columns">
      <div class="column left">
        <div class="heading">
          <div class="background-circle"></div>
          <p>Hi I'm John</p>
        </div>
        <div class="subheading">
          Full stack Software Developer with a passion for design and creating
          useful user experiences
        </div>
        <div class="button-wrap"><button>Let's Chat</button></div>
        <div class="social-buttons">
          <div class="button linkedin"></div>
          <div class="button twitter"></div>
          <div class="button instagram"></div>
          <div class="button github"></div>
        </div>
      </div>
      <div class="column right">
        <div class="image-wrap">
          <div class="image"></div>
        </div>
      </div>
    </div>
    <!--<img alt="Vue logo" src="../assets/logo.png" />-->
  </div>
</template>

<script>
import MenuBar from "@/components/common/MenuBar.vue";

export default {
  name: "HomeView",
  components: { MenuBar },
};
</script>

<style lang="scss" scoped>
p {
  margin: 0;
  padding: 0;
}
.home-view {
  height: 100vh;
}
.top-bar {
  height: 100px;
  display: grid;
  grid-template-columns: 1fr 2fr 3fr;
}
.top-bar .logo {
  display: flex;
  justify-content: center;
  align-content: center;
  align-items: center;
  font-size: 2rem;
  font-weight: 600;
}
.columns {
  display: grid;
  grid-template-columns: 1.5fr 1fr;
  width: 100%;
  height: calc(100vh - 100px);
}
.column.left {
  position: relative;
  padding: 150px 80px;
  display: grid;
  grid-template-rows: 1fr 1fr 1fr 1fr 1fr;
  max-width: 650px;
  gap: 10px;
}
.column.right {
  padding: 110px 0px;
}
.background-circle {
  position: absolute;
  top: -30px;
  right: 35%;
  width: 100px;
  height: 100px;
  border-radius: 50px;
  background: linear-gradient(
    163.24deg,
    #dc9521 34.15%,
    rgba(163, 155, 41, 0.93) 95.22%
  );
  z-index: 1;
}
.heading {
  font-size: 4rem;
  font-weight: 700;
  text-align: left;
  padding: 0px 50px;
  position: relative;
}
.heading p {
  z-index: 1;
  position: relative;
}
.subheading {
  font-size: 1.2rem;
  font-weight: 500;
  text-align: left;
  padding: 0px 50px;
}
.button-wrap {
  text-align: left;
  padding: 0px 50px;
}
.button-wrap button {
  padding: 20px 50px;
  border-radius: 10px;
  background-color: #d89623;
  font-size: 1.4rem;
  font-weight: 600;
  cursor: pointer;
  box-shadow: 7px 7px 20px 3px #d3d3d3;
}
.social-buttons {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  padding: 0px 50px;
  gap: 30px;
}
.social-buttons .button {
  width: 100%;
  aspect-ratio: 1;
  border-radius: 50%;
  cursor: pointer;
  background-color: #d89623;
  background-size: 65%;
  background-repeat: no-repeat;
  background-position: center;
  max-width: 80px;
}
.button.linkedin {
  background-image: url("https://img.icons8.com/ios-glyphs/90/000000/linkedin-circled--v1.png");
}
.button.twitter {
  background-image: url("https://img.icons8.com/ios-glyphs/90/000000/twitter-circled--v1.png");
}
.button.instagram {
  background-image: url("https://img.icons8.com/ios-glyphs/90/000000/instagram-new.png");
}
.button.github {
  background-image: url("https://img.icons8.com/ios-glyphs/90/000000/github.png");
}
.image-wrap {
  width: 600px;
  height: 600px;
  position: relative;
}
.image-wrap .image {
  background-image: url(http://localhost:8080/img/body_shot.760d3902.jpeg);
  width: 100%;
  height: 100%;
  background-size: 100%;
  background-repeat: no-repeat;
  background-position: center;
  position: absolute;
  top: 0px;
  right: -25%;
  border-radius: 20%;
}
</style>
