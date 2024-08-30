<template>
  <div>
    <primeiroComponente/>
    <p> {{ testando }}</p>
  </div>
</template>

<script>
  import primeiroComponente from './components/primeiroComponente.vue'
  
  export default {
    name: 'App',
    components: {
      primeiroComponente
    },
    data() {
      return {
        testando : "Test"
      }
    }
  }
</script>