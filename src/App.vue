<template>
  <div class="min-vh-100 bg-light">
    <nav class="navbar navbar-dark bg-primary mb-4">
      <div class="container">
        <span class="navbar-brand mb-0 h1">Vue + Bootstrap Demo</span>
      </div>
    </nav>

    <div class="container py-4">
      <div class="row mb-5">
        <div class="col-lg-8 mx-auto">
          <h2 class="h4 mb-3">Perfil de Usuario</h2>
          <UserProfile />
        </div>
      </div>

      <div class="row mb-5">
        <div class="col-lg-10 mx-auto">
          <h2 class="h4 mb-3">Catálogo de Productos</h2>
          <Product />
        </div>
      </div>

      <div class="row mb-5">
        <div class="col-lg-6 mx-auto">
          <h2 class="h4 mb-3">Registro de Usuario</h2>
          <FormularioUsuario />
        </div>
      </div>

      <div class="row">
        <div class="col-12">
          <h2 class="h4 mb-3">Lista de Productos</h2>
          <ListaProductos :productos="productosData" />
        </div>
      </div>
    </div>

    <footer class="bg-dark text-white py-4 mt-5">
      <div class="container text-center">
        <p class="mb-0">
          © 2024 Vue + Bootstrap Demo. Todos los derechos reservados.
        </p>
      </div>
    </footer>
  </div>
</template>

<script>
import UserProfile from "./components/UserProfile.vue";
import Product from "./components/Product.vue";
import FormularioUsuario from "./components/FormularioUsuario.vue";
import ListaProductos from "./components/ListaProductos.vue";

export default {
  name: "App",
  components: {
    UserProfile,
    Product,
    FormularioUsuario,
    ListaProductos,
  },
  data() {
    return {
      productosData: [
        {
          id: 1,
          nombre: "MacBook Pro",
          precio: 1299.99,
          categoria: "Laptops",
          stock: 10,
        },
        {
          id: 2,
          nombre: "iPhone 13",
          precio: 999.99,
          categoria: "Smartphones",
          stock: 15,
        },
        {
          id: 3,
          nombre: "iPad Air",
          precio: 599.99,
          categoria: "Tablets",
          stock: 8,
        },
        {
          id: 4,
          nombre: "AirPods Pro",
          precio: 249.99,
          categoria: "Accesorios",
          stock: 20,
        },
        {
          id: 5,
          nombre: "Apple Watch",
          precio: 399.99,
          categoria: "Wearables",
          stock: 12,
        },
      ],
    };
  },
};
</script>
