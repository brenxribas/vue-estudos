<template>
  <BannerVue />
  <div class="main-container">
    <h1>Monte seu burger</h1>
    <p>Formulário</p>
  </div>
</template>

<script>
import BannerVue from "../components/Banner.vue";

export default {
  name: 'Home',
  components: {
    BannerVue
  }
};
</script>

<style scoped>
</style>