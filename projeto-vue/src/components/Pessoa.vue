<template>
  <div>
    <h2>Esta é a descrição da pessoa: {{ nome }}</h2>
    <InfoVue/>
    <FormVue />
  </div>
</template>

<script>

import InfoVue from './Info.vue';
import FormVue from './Form.vue';

export default {
  name: "Pessoa",
  components: {
    data() {
      InfoVue,
      FormVue
    },
  },
  data() {
    return {
      nome: "Breno",
    };
  },
  components: { InfoVue, FormVue },
};
</script>