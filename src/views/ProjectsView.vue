<template>
  <div class="projects-view">
    <div class="top-bar">
      <div class="logo">JPM</div>
      <div class="spacer"></div>
      <div class="menu">
        <menu-bar></menu-bar>
      </div>
    </div>
  </div>
</template>

<script>
import MenuBar from "@/components/common/MenuBar.vue";

export default {
  name: "ProjectsView",
  components: { MenuBar },
  methods: {},
};
</script>

<style scoped>
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
</style>
