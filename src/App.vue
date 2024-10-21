<script>
import UserProfile from './components/UserProfile.vue';
import Product from './components/Product.vue';
import FormularioUsuario from './components/FormularioUsuario.vue';
import ListaProductos from './components/ListaProductos.vue';

export default {
    name: 'App',
    components: {
        UserProfile,
        Product,
        FormularioUsuario,
    },
    data() {
        return {
            productos: [
                { id: 1, nombre: 'GTA 5', precio: 15000 },
                { id: 2, nombre: 'GTA 4', precio: 8000 },
                { id: 3, nombre: 'GTA III', precio: 5000 },
            ],
        };
    },
};
</script>

<template>
    <div class="container mt-5">
        <h1 class="mb-4">Ejercicios Vue con Bootstrap</h1>

        <h2 clas="mb-3">Ejercicio 1: Perfil de Usuario</h2>
        <UserProfile />

        <h2 clas="mb-3">Ejercicio 2: Productos</h2>
        <Product />

        <h2 clas="mb-3">Ejercicio 3: Formulario de Usuario</h2>
        <FormularioUsuario />

        <h2 clas="mb-3">Ejercicio 4: Lista de productos con props y Bootstrap</h2>
        <ListaProductos :productos="productos" />
    </div>
</template>
