<script>
export default {
    name: 'FormularioUsuario',
    data() {
        return {
            nombre: '',
            edad: '',
        };
    },
};
</script>

<template>
    <form>
        <div class="mb-3">
            <label for="exampleInputEmail1" class="form-label">Nombre</label>
            <input type="text" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" v-model="nombre" />
        </div>
        <div class="mb-3">
            <label for="exampleInputPassword1" class="form-label">Edad</label>
            <input type="number" class="form-control" id="exampleInputPassword1" v-model="edad" />
        </div>
        <button type="submit" class="btn btn-primary">Limpiar</button>
        <hr />
        <p>Nombre: {{ nombre }}</p>
        <p>Edad: {{ edad }}</p>
    </form>
</template>

<style scoped></style>
