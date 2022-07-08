<!-- LIFECYCLE HOOKS  -->
<template>
  <div>
    <h1>Meu nome é: {{ nome }}</h1>
  </div>
</template>

<script>
export default {
  name: "LifeCycle",
  data() {
    return {
      nome: "Ainda não sei",
    };
  },
  created() {
    setTimeout(() => {
      this.nome = "Breno";
    }, 1000);
    this.lifeCycle();
  },
  mounted() {
    setTimeout(() => {
      this.nome = "Pedro";
    }, 3000);
  },
  methods: {
    lifeCycle() {
      console.log("Testando");
    },
  },
};
</script>