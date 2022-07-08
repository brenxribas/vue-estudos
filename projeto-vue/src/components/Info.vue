<template>
  <div>
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oportunidades.</p>
    <p>Utilizo as seguintes tecnologias:</p>

    <ul>
      <li>Javascript</li>
      <li>Node.js</li>
      <li>Vue.js</li>
    </ul>

    <button @click="showEmail">{{textoBotao}}</button>
    <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>

    <p>Para acessar meu portifólio basta <a v-bind:href="meu_link">clicar aqui</a></p>
    <PictureVue />

  </div>
</template>

<script>
import PictureVue from "./Picture.vue";

export default {
  name: "Info",
  data() {
    return {
      esta_trabalhando: false,
      mostrar_email: false,
      email: "breno_ribas@outlook.com",
      meu_link: "https://google.com",
      textoBotao: "Mostrar email"
    };
  },
  components: {
    PictureVue,
  },
  methods: {
    showEmail(){
      this.mostrar_email = !this.mostrar_email
      if(!this.mostrar_email){
        this.textoBotao = "Mostrar email"
      }else{
        this.textoBotao = "Esconder email"
      }
    }
  },
};
</script>
