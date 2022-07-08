<template>
  <div>
    <h2>Esta é a descrição da pessoa: {{ nome }}</h2>
    <InfoVue :email="email" :esta_trabalhando=false />
    <FormVue />
  </div>
</template>

<script>
import InfoVue from "./Info.vue";
import FormVue from "./Form.vue";

export default {
  name: "Pessoa",
  components: {
    InfoVue,
    FormVue,
  },
  data() {
    return {
      nome: "Programador Fullstack",
      email: "breno@email.com",
    };
  },
  components: { InfoVue, FormVue },
};
</script>