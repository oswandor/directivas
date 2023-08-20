<template>
  <div class="container">

    <h1>Directivas Basicas</h1>
    <Directiva></Directiva>
    <DirectivasCondicionales></DirectivasCondicionales>

  </div>
</template>

<script>
import Directiva from './components/Directiva.vue'
import DirectivasCondicionales from './components/DirectivasCondicionales.vue';

export default {
  name: 'App',
  components: {
    Directiva,
    DirectivasCondicionales
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
