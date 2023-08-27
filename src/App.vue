<template>
  <div class="container">

    <h1>Directivas Basicas</h1>
    <DirectivaBind></DirectivaBind>
    <DirectivasItererativas></DirectivasItererativas>

  </div>
</template>

<script>
import Directiva from './components/Directiva.vue'
import DirectivaBind from './components/DirectivaBind.vue';
import  DirectivasItererativas from './components/DirectivasItererativas.vue';


export default {
  name: 'App',
  components: {
    DirectivaBind , 
    DirectivasItererativas
  }
}
</script>

<style>
.container {
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  color: blue;
  padding: 10px;
}
</style>
