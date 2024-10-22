<template>
  <div class="card h-100 shadow-sm">
    <div
      class="badge bg-danger position-absolute end-0 m-2"
      v-if="producto.stock < 10"
    >
      ¡Pocas unidades!
    </div>
    <div class="card-body">
      <h5 class="card-title text-primary">{{ producto.nombre }}</h5>
      <p class="card-text text-muted mb-1">{{ producto.categoria }}</p>
      <div class="d-flex justify-content-between align-items-center mb-2">
        <span class="fs-4 fw-bold text-success">${{ producto.precio }}</span>
        <span class="badge bg-info">Stock: {{ producto.stock }}</span>
      </div>
      <div class="d-grid gap-2">
        <button class="btn btn-outline-primary">
          <i class="bi bi-cart-plus me-2"></i>Agregar al carrito
        </button>
        <button class="btn btn-outline-secondary btn-sm">Ver detalles</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProductoItem",
  props: {
    producto: {
      type: Object,
      required: true,
    },
  },
};
</script>
