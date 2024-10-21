<<<<<<< HEAD
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
=======
<script setup>
import FormularioUsuario from './components/FormularioUsuario.vue';
</script>

<template>
    <FormularioUsuario />
>>>>>>> 2e5be8a82c3b05a79a56b6e7111db071fca46bc9
</template>

<style scoped></style>
