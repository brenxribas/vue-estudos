<template>
  <div class="main-container">
    <h1>Pedidos</h1>
    <DashboardVue />
  </div>
</template>

<script>
import DashboardVue from "@/components/Dashboard.vue";

export default {
  name: "Pedidos",
  components: {
    DashboardVue
  }
};
</script>