
<template lang="es">
    <div>
                
        <p v-if="promedio >= 7 ">
        
            Usted a aprobado el promedio Final: {{ promedio }}

        </p>

        <h3>Condicional v-else</h3> 
        <p id="par" v-if="numero%2===0">El numero {{ numero }} es par.</p>
        
        <p id="impar" v-else > El numero {{ numero }} es impar.</p>


        <h3>Condicional multiple</h3>


        <p v-if="num===0">
        numero es {{ num }} es cero 
        </p>

        <p v-else-if="num>0"> Numero es Positivo {{ num }}</p> 

        <p v-else> 

            numero es distinto 
        </p>


        <h3>Mostrar v-show</h3>

        <p v-show="login">Sesion iniciada</p>

    </div>
</template>
<script>
export default {
    name: "DirectivasCondicionales",
    data() {

        return {

            promedio: 7,
            numero: 5, 
            num:0 , 
            login:true , 
        }
    }
}
</script>
<style scoped >
    #par{

        color: blue; 
    }

#impar {
    color:green; 
}

h3 {

    color: black;
}

h1 {

color: black;
}
</style>