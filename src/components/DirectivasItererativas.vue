<template >
    <h1>Directiva For</h1>
    <br><br>
    <h2>Lista de Pacientes</h2>
    <br>

    <ul>
        <li v-for="(pais, index) in paises" :key="index">
            {{ pais }}
        </li>
    </ul>
    <br>
    <h2>Listado de colores</h2>
    <select name="" id="">

        <option v-for="(color, index) in colores" :key="index" value="index">
            {{ color }}
        </option>
    </select>

    <br><br>
    <hr>
    <h1>Directiva For en arreglo de objetos</h1>
    <h2>Talba de Pa&iacute;ses</h2>

    <table>
        <tr>
            <th>Pa&iacute;s</th>
            <th>Capital</th>
        </tr>

        <tr v-for="pais in paisesObj" :key="pais.code">

            <td>{{ pais.nombre }}</td>

            <td>{{ pais.capital }}</td>



        </tr>
    </table>

    <br><br>
    <hr>

    <h1>Directiva For en Objetos</h1>
    <h2>Propiedades de Objetos</h2>

    <ul>
        <li v-for="(valor, propiedad) in objeto " :key="valor"> {{ propiedad }}: {{ valor }} </li>
    </ul>
</template>
<script>
export default {
    name: 'DirectivasItererativas',
    data() {

        return {
            paises: ['El salvador', 'España', 'Estados Unidos'],
            colores: ['Blanco', 'Negro', 'Rojo'],
            paisesObj: [
                { code: 1, nombre: 'El salvador', capital: 'San Salvador' },
                { code: 2, nombre: 'España', capital: 'Madrid' },
                { code: 3, nombre: 'Francia', capital: 'Paris' },
            ],
            objeto: {

                tipo: 'Gato',
                nombre: 'KidMinino',
                edad: 3
            }
        }

    }
}
</script>
<style>
h2,
ul {
    color: #3F2305;
}

table {
    color: #001C30;
    border-collapse: collapse;
}

td {
    border: 1px solid #001C30;
}
</style>