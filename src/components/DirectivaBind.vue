<template>
    <div>
        <h1>Directiva v-bind</h1>
        <img :src="imagen" v-bind:alt="texto">
    </div>

    <br><br><hr>

    <h1>Directiva v-bind para clases y estilos css</h1>
    <p>Hola mundo desde vue</p>

    <p v-bind:class="classColor" :style="styles">Hola Mundo desde vue</p>
    <br><br><hr>

    <div class="container">
        <h1>Directiva v-on</h1>

        <button v-on:click="saludar">Boton 1</button>
        
        <button @click="saludar">Boton 2</button>

    </div>


</template>
<script>
export default {

    name: 'DirectivaBind',
    data() {

        return{
            imagen: 'https://picsum.photos/200/300',
            texto: 'Texto de la imagen' , 
            classColor:'text' , 
            styles:{
                'font-size': '2em' , 
                'font-weight': 'bold' , 
                'backgroud-color': '#ECF8F9', 
            }
        };
    }, 
    methods:{

        saludar(){

                alert("Hola mundo desde Vue.js")
        }

    }
}
</script>
<style>
    .text{
        color:green; 
        text-align: center; 
    }
</style>