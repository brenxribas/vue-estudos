<template>
  <div>
    <img :src="avatar" :alt="descricao" />
    <MudarImagemVue @mudar-imagem="trocarImagem" />
  </div>
</template>

<script>
import MudarImagemVue from "./MudarImagem.vue";
import ReutilizacaoVue from "./Reutilizacao.vue";
export default {
  name: "Picture",
  data() {
    return {
      avatar: "/img/avatar.png",
      descricao: "Breno Ribas",
    };
  },
  components: {
    ReutilizacaoVue,
    MudarImagemVue,
  },
  methods: {
    trocarImagem() {
      this.avatar = "img/avatar2.png";
    },
  },
};
</script>