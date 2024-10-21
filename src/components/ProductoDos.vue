<script>
export default {
    name: 'ProductoDos',
    props: {
        producto: {
            type: Object,
            required: true,
        },
    },
};
</script>

<template>
    <div class="card">
        <div class="card-body">
            <h5 class="card-title">{{ producto.nombre }}</h5>
            <p class="card-text">${{ producto.precio }}</p>
        </div>
    </div>
</template>

<style scoped></style>
