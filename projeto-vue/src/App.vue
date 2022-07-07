<template>
  <div>
    <PrimeiroComponenteVue />
    <LifeCycleVue />
    <PessoaVue/>
  </div>
</template>

<script>
import PrimeiroComponenteVue from "./components/PrimeiroComponente.vue";
import LifeCycleVue from "./components/LifeCycle.vue";
import PessoaVue from "./components/Pessoa.vue";

export default {
  name: "App",
  components: {
    PrimeiroComponenteVue,
    LifeCycleVue,
    PessoaVue
  },
  data() {
    return {

    };
  },
};
</script>

<!-- <template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style> -->
