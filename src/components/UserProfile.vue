<template>
  <div class="card" style="width: 18rem">
    <div class="card-body">
      <h5 class="card-title">{{ nombre }}</h5>
      <h6 class="card-subtitle mb-2 text-muted">{{ email }}</h6>
      <p class="card-text">{{ bio }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "UserProfile",
  data() {
    return {
      nombre: "Juan Rojas",
      email: "juanrojas@yahoo.com",
      bio: "Apasionado corredor de F1",
    };
  },
};
</script>

<style scoped></style>
