<template>
  <div>
    
    <NavbarVue :logo="logo_src" :alt="app_name"/>
    <router-view />
    <FooterVue />

  </div>
</template>

<script>
import NavbarVue from "./components/Navbar.vue";
import FooterVue from "./components/Footer.vue";

export default {
  components: {
    NavbarVue,
    FooterVue
  },
  data() {
    return {
      logo_src: "/img/logo.png",
      app_name: "Make your Burger"
    }
  },
};
</script>

<style>
* {
  font-family: Helvetica, sans-serif;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.main-container{
  margin: 50px;
  min-height: 250px;
}

h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 50px;
  color: #222;
}
</style>
