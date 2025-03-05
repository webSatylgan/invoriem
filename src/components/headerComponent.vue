<script setup>

import Button from "@components/ui/Button.vue";
</script>

<template>
  <div class="header">
    <div class="container">
      <div class="header_container flex">
        <img src="@assets/imgs/logo.svg" alt="" id="logo">
        <nav>
          <a href="">About us</a>
          <Button>Let’s Talk</Button>
        </nav>
      </div> <!-- header_container -->
    </div> <!-- container -->
  </div> <!-- Header -->
</template>

<style scoped>
  .header {
    width: 100%;
    padding: 45px 0;

    position: absolute;
    top: 0;
    left: 0;
    z-index: 10;
  }

  .header_container > nav {
    max-width: 420px;
    padding: 0 10px;
  }

  @media (max-width: 1000px) {
      .header_container nav {
          max-width: 300px;
      }
  }
  
  @media (max-width: 600px) {
      .header_container nav {
          display: none;
      }
  }

</style>