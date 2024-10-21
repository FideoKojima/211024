<template>
  <div class="list-group">
    <div clas="list-group-item">
      <h5>{{ nombre }}</h5>
      <p :style="{ color: precioColor }">Precio: ${{ precio }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Product",
  data() {
    return {
      nombre: "Laptop",
      precio: 1000,
      precioColor: "green",
    };
  },
};
</script>

<style scoped></style>
