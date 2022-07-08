<template>
  <div>
    <PictureVue />

    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oportunidades.</p>
    
    <p>Utilizo as seguintes tecnologias para back-end:</p>
    <ul>
      <li v-for="(technology, index) in backend_tecnologies" v-bind:key="index">{{technology}}</li>
    </ul>

    <p>Utilizo as seguintes tecnologias para front-end:</p>
    <ul>
      <li v-for="technology in frontend_tecnologies" :key="technology.id">{{technology.language}}</li>
    </ul>

    <button @click="showEmail">{{ textoBotao }}</button>
    <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>

    <p>
      Para acessar meu portifólio basta
      <a v-bind:href="meu_link">clicar aqui</a>
    </p>
   
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
      textoBotao: "Mostrar email",
      backend_tecnologies: ["Javascript", "PHP", "Python"],
      frontend_tecnologies: [
        {id: 1, language: 'HTML5'},
        {id: 2, language: 'CSS3'},
        {id: 3, language: 'React'}
      ]
    };
  },
  components: {
    PictureVue,
  },
  methods: {
    showEmail() {
      this.mostrar_email = !this.mostrar_email;
      if (!this.mostrar_email) {
        this.textoBotao = "Mostrar email";
      } else {
        this.textoBotao = "Esconder email";
      }
    },
  },
};
</script>

<style scoped>
ul {
  list-style: none; 
}
 
li {
  margin-top: 10px;
  margin-right: 20px;
}

</style>