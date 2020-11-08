<template>
  <div id="app">
    <entete/>
    <contenu/>
    <tableau/>
  </div>
</template>

<script>
import entete from './components/entete.vue'
import tableau from './components/tableau.vue'
import contenu from './components/contenu.vue'


export default {
  name: 'App',
  components: {
    entete,
    tableau,
    contenu
  }
}
</script>

<style>

</style>
