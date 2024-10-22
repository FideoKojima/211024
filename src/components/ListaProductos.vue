<template>
  <div>
    <div class="d-flex justify-content-between align-items-center mb-4">
      <div class="d-flex gap-3 align-items-center">
        <div class="input-group" style="width: 300px">
          <span class="input-group-text">
            <i class="bi bi-search"></i>
          </span>
          <input
            type="text"
            class="form-control"
            placeholder="Buscar productos..."
          />
        </div>
        <select class="form-select" style="width: 200px">
          <option value="">Todas las categorías</option>
        </select>
      </div>
      <span class="badge bg-secondary">
        {{ productos.length }} productos encontrados
      </span>
    </div>

    <div class="row g-4">
      <div v-for="producto in productos" :key="producto.id" class="col-md-4">
        <ProductoItem :producto="producto" />
      </div>
    </div>
  </div>
</template>

<script>
import ProductoItem from "./ProductoItem.vue";

export default {
  name: "ListaProductos",
  components: {
    ProductoItem,
  },
  props: {
    productos: {
      type: Array,
      required: true,
      default: () => [],
    },
  },
};
</script>
