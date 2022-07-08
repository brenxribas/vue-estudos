<template>
  <div>
    <h1>Hello Vue!</h1>
    <p>Meu nome é {{ name }} e trabalho como {{ profissao }}</p>
    <MultiplosEventosVue/>
  </div>
</template>

<script>
import MultiplosEventosVue from './MultiplosEventos.vue';
MultiplosEventosVue

export default {
  name: "PrimeiroComponente",
  data() {
    return {
      name: "Breno",
      profissao: "Programador"
    };
  },
  components: {
    MultiplosEventosVue
  }
};
</script>