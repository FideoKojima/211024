<script>
import ProductoDos from './ProductoDos.vue';
export default {
    name: 'ListaProductos',
    components: {
        ProductoDos,
    },
    props: {
        productos: {
            type: Array,
            required: true,
        },
    },
};
</script>

<template>
    <div>
        <div class="row">
            <div class="col-md-4" v-for="producto in productos" :key="producto.id">
                <ProductoDos :producto="producto" />
            </div>
        </div>
    </div>
</template>

<style scoped></style>
