<template>
  <div>
    <h2>Meu formulário: </h2>
    <form action="">
      <div><InputTextVue /></div>
      <div><InputTextVue /></div>
      <div><SubmitVue /></div>
    </form>
  </div>
</template>

<script>
import InputTextVue from "./form/InputText.vue";
import SubmitVue from "./form/Submit.vue";

export default {
  name: "Form",
  components: {
    InputTextVue,
    SubmitVue,
  },
};
</script>