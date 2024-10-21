<script>
import UserProfile from "./components/UserProfile.vue";
import Product from "./components/Product.vue";
import FormularioUsuario from "./components/FormularioUsuario.vue";

export default {
  name: "App",
  components: {
    UserProfile,
    Product,
    FormularioUsuario,
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

    <h2 clas="mb-3">Ejercicio 3: Formulario de Usuario</h2>
    <FormularioUsuario />
  </div>
</template>
```
