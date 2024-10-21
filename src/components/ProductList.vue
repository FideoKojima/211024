<template>
  <div class="row">
    <div v-for="producto in productos" :key="producto.id" class="col-md-4 mb-3">
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">{{ producto.nombre }}</h5>
          <p class="card-text">Precio: ${{ producto.precio }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ListaProductos",
  data() {
    return {
      productos: [
        { id: 1, nombre: "Producto A", precio: 19.99 },
        { id: 2, nombre: "Producto B", precio: 29.99 },
        { id: 3, nombre: "Producto C", precio: 39.99 },
      ],
    };
  },
};
</script>
