<template>
  <div>
    <h1>Hello Vue!</h1>
    <p>Meu nome é {{ name }} e trabalho como {{ profissao }}</p>
    <MultiplosEventosVue/>
    <ReutilizacaoVue/>
    <ReutilizacaoVue/>
    <ReutilizacaoVue/>
    <ReutilizacaoVue/>
    
  </div>
</template>

<script>
import MultiplosEventosVue from './MultiplosEventos.vue';
import ReutilizacaoVue from './Reutilizacao.vue';

export default {
  name: "PrimeiroComponente",
  data() {
    return {
      name: "Breno",
      profissao: "Programador"
    };
  },
  components: {
    MultiplosEventosVue,
    ReutilizacaoVue
  }
};
</script>