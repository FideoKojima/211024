<script>
import UserProfile from "./components/UserProfile.vue";
import Product from "./components/Product.vue";

export default {
  name: "App",
  components: {
    UserProfile,
    Product,
  },
};
</script>

<template>
  <div class="container mt-5">
    <h1 class="mb-4">Ejercicios Vue con Bootstrap</h1>

    <h2 clas="mb-3">Ejercicio 1: Perfil de Usuario</h2>
    <UserProfile />

    <h2 clas="mb-3">Ejercicio 2: Productos</h2>
    <Product />
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
