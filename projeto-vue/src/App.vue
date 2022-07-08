<template>
  <div>
    <HeaderVue/>
    <PrimeiroComponenteVue />
    <LifeCycleVue />
    <PessoaVue/>
  </div>
</template>

<script>
import HeaderVue from './components/Header.vue';
import PrimeiroComponenteVue from "./components/PrimeiroComponente.vue";
import LifeCycleVue from "./components/LifeCycle.vue";
import PessoaVue from "./components/Pessoa.vue";

export default {
  name: "App",
  components: {
    HeaderVue,
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

<style>

body {
  background-color: darkslateblue;
  color: white;
  text-align: center;
  font-size: 16px;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

</style> -->
