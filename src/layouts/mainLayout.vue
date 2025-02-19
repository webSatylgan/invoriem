<script setup>

  import HeaderComponent from "@components/headerComponent.vue";
  import FooterComponent from "@components/footerComponent.vue";
</script>

<template>
  <header-component />
    <slot></slot>
  <footer-component />
</template>

<style scoped>

</style>