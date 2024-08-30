<template>
  <div>
    <primeiroComponente/>
    <p> {{ testando }}</p>
    <LifeCycle />
    <pessoa />
  </div>
</template>

<script>

import PrimeiroComponente from './components/PrimeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';

  
  export default {
    name: 'App',
    components: {
      PrimeiroComponente,
      // eslint-disable-next-line vue/no-unused-components
      LifeCycle,
      Pessoa
    },
    data() {
      return {
        testando : "Test"
      }
    }
  }
</script>