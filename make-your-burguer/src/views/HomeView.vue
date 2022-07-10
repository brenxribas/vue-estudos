<template>
  <BannerVue />
  <div class="main-container">
    <h1>Monte seu burger</h1>
    <BurguerFormVue/>
  </div>
</template>

<script>
import BurguerFormVue from '@/components/BurguerForm.vue';
import BannerVue from "../components/Banner.vue";

export default {
  name: 'Home',
  components: {
    BannerVue,
    BurguerFormVue
  }
};
</script>

<style scoped>
</style>