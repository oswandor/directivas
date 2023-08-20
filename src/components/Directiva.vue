<template>
    <h3> Directiva v-text</h3>
    <p>{{ texto }}</p>
    <p v-text="texto"></p>

    <h3>Directiva vu-html</h3>

    <p v-html="html"></p>


    <h3>Directiva V-model</h3>

    Libro: <input type="text" v-model="libro">

    Descripcion: <textarea name="" id="" cols="10" rows="2" v-model="descripcion"></textarea>
</template>
<script>


export default {
    name: 'Directiva',
    data() {

        return {

            texto: 'Hola mundo soy un Texto',
            html: '<a href="https://google.com">google</a>',
            libro: 'UML 24 HORAS',
            descripcion: 'Este es un libro para aprender analisis'
        }
    }
}
</script>
<style>

h3{

    color: black;
}

</style>