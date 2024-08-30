<template>
  <div>
    <primeiroComponente/>
    <p> {{ testando }}</p>
    <LifeCycle />
  </div>
</template>

<script>

import PrimeiroComponente from './components/PrimeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue'

  
  export default {
    name: 'App',
    components: {
      PrimeiroComponente,
      // eslint-disable-next-line vue/no-unused-components
      LifeCycle
    },
    data() {
      return {
        testando : "Test"
      }
    }
  }
</script>