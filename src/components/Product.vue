<template>
  <div class="list-group">
    <div
      v-for="producto in productos"
      :key="producto.id"
      class="list-group-item"
    >
      <h5>{{ producto.nombre }}</h5>
      <p :style="{ color: producto.precioColor }">
        Precio: ${{ producto.precio.toFixed(2) }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Producto",
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
