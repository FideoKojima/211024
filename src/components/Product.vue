<template>
  <div class="list-group shadow-sm">
    <div
      v-for="producto in productos"
      :key="producto.id"
      class="list-group-item list-group-item-action d-flex justify-content-between align-items-center"
    >
      <div>
        <h5 class="mb-1">{{ producto.nombre }}</h5>
        <p class="mb-1" :style="{ color: producto.precioColor }">
          <strong>${{ producto.precio.toFixed(2) }}</strong>
        </p>
      </div>
      <div class="d-flex gap-2">
        <span class="badge bg-success rounded-pill">En Stock</span>
        <button class="btn btn-outline-primary btn-sm">
          Agregar al carrito
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Product",
  data() {
    return {
      productos: [
        {
          id: 1,
          nombre: "Smartphone XYZ",
          precio: 599.99,
          precioColor: "green",
        },
        { id: 2, nombre: "Laptop ABC", precio: 1299.99, precioColor: "blue" },
        { id: 3, nombre: "Tablet 123", precio: 399.99, precioColor: "red" },
        {
          id: 4,
          nombre: "Smartwatch QWE",
          precio: 199.99,
          precioColor: "purple",
        },
        {
          id: 5,
          nombre: "Auriculares Bluetooth",
          precio: 79.99,
          precioColor: "orange",
        },
      ],
    };
  },
};
</script>
