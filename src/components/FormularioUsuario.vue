<template>
  <div class="card shadow-sm">
    <div class="card-header bg-success text-white">
      <h5 class="mb-0">Registro de Usuario</h5>
    </div>
    <div class="card-body">
      <form>
        <div class="mb-3">
          <label for="nombre" class="form-label">Nombre:</label>
          <div class="input-group">
            <span class="input-group-text">
              <i class="bi bi-person"></i>
            </span>
            <input
              type="text"
              class="form-control"
              id="nombre"
              v-model="nombre"
              placeholder="Ingrese su nombre"
            />
          </div>
        </div>
        <div class="mb-3">
          <label for="edad" class="form-label">Edad:</label>
          <div class="input-group">
            <span class="input-group-text">
              <i class="bi bi-calendar"></i>
            </span>
            <input
              type="number"
              class="form-control"
              id="edad"
              v-model="edad"
              placeholder="Ingrese su edad"
            />
          </div>
        </div>
        <div class="d-grid gap-2">
          <button type="submit" class="btn btn-success">Guardar Datos</button>
        </div>
      </form>
      <div class="mt-4 p-3 bg-light rounded">
        <h6 class="text-muted mb-2">Datos Ingresados:</h6>
        <p class="mb-1">
          <strong>Nombre:</strong> {{ nombre || "No especificado" }}
        </p>
        <p class="mb-0">
          <strong>Edad:</strong> {{ edad || "No especificada" }}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FormularioUsuario",
  data() {
    return {
      nombre: "",
      edad: null,
    };
  },
};
</script>
