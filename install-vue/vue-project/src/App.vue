<template>
  <div>
    <Header :esta_logado=true />
    <primeiroComponente/>
    <p class="paragrafo-pai">O dados de app é: {{ testando }}</p>
    <LifeCycle />
    <pessoa />
  </div>
</template>

<script>

import PrimeiroComponente from './components/PrimeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';
import Header from './components/Header.vue';

  
  export default {
    name: 'App',
    components: {
      PrimeiroComponente,
      // eslint-disable-next-line vue/no-unused-components
      LifeCycle,
      Pessoa,
      // eslint-disable-next-line vue/no-reserved-component-names
      Header
    },
    data() {
      return {
        testando : "Test"
      }
    }
  }
</script>

<style>
  body {
    background-color: black;
    color: white;
  }

  a {
    color: aqua;
  }

  .test {
    color: blueviolet;
  }
</style>