<template>
  <nav class="nav-bar">
    <router-link to="/">Home</router-link>
  </nav>
</template>

<script>
export default {};
</script>

<style scoped>
nav {
  padding: 30px;
}
nav a {
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
}
nav a.router-link-exact-active {
  color: #bd7800;
}
.nav-bar {
  display: flex;
  gap: 40px;
  justify-content: center;
}
</style>
