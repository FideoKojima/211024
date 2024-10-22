<template>
  <div class="card shadow-sm">
    <div class="card-header bg-primary text-white">
      <h5 class="mb-0">Perfil de Usuario</h5>
    </div>
    <div class="card-body">
      <div class="d-flex align-items-center mb-3">
        <div class="bg-light rounded-circle p-3 me-3">
          <i class="bi bi-person-circle fs-1"></i>
        </div>
        <div>
          <h5 class="card-title mb-1">{{ nombre }}</h5>
          <h6 class="card-subtitle text-muted">{{ ocupacion }}</h6>
        </div>
      </div>
      <p class="card-text border-top pt-3">{{ biografia }}</p>
      <div class="d-flex justify-content-end">
        <button class="btn btn-outline-primary btn-sm">Editar Perfil</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "UserProfile",
  data() {
    return {
      nombre: "Juan Pérez",
      ocupacion: "Desarrollador Web",
      biografia:
        "Apasionado por la tecnología y el desarrollo de aplicaciones web innovadoras. Especializado en Vue.js y desarrollo frontend.",
    };
  },
};
</script>
