<template>
  <div class="list-group">
    <div clas="list-group-item">
      <h5>{{ nombre }}</h5>
      <h5>{{ nombre2 }}</h5>
      <h5>{{ nombre3 }}</h5>

      <p :style="{ color: precioColor }">Precio: ${{ precio }}</p>
      <p :style="{ color: precioColor2 }">Precio: ${{ precio2 }}</p>
      <p :style="{ color: precioColor3 }">Precio: ${{ precio3 }}</p>
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

      nombre2: "Smartphone",
      precio2: 500,
      precioColor2: "red",

      nombre3: "Tablet",
      precio3: 300,
      precioColor3: "blue",
    };
  },
};
</script>

<style scoped></style>
