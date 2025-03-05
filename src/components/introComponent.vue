<script setup>

import Button from "@components/ui/Button.vue";
</script>

<template>
  <div class="intro">
    <div class="container">
      <div class="intro_container">
        <h1>We build dreams, <br> not just walls</h1>
        <p>Fulfill your international property developments with us</p>
        <Button>Let’s Talk</Button>
      </div>
    </div>
    <svg class="intro_arrows" viewBox="0 0 39 30" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M0.5 1L19.5 20L38.5 1" />
      <path d="M0.5 10L19.5 29L38.5 10" />
    </svg>
  </div> <!-- intro -->
</template>

<style scoped>
  .intro {
    width: 100%;
    height: 100vh;
    background: url("@assets/imgs/intro.png") center/cover no-repeat;

    position: relative;
  }

  .intro_arrows {
    width: 40px;
    height: 30px;

    position: absolute;
    bottom: 60px;
    left: 50%;
    transform: translateX(-50%);

    stroke: #fff;

    cursor: pointer;
    transition: .2s;
  }

  .intro_arrows:hover {
    stroke: var(--teal);
  }

  .intro_container {
    display: flex;
    align-items: flex-start;
    flex-direction: column;
    justify-content: center;

    width: 100%;
    height: 100vh;
  }

  .intro_container p {
    margin-top: 50px;

    font-family: var(--Work-family);
    font-size: 34px;
    letter-spacing: -0.02em;
  }


  .intro_container button {
    margin-top: 72px;

    color: #fff;
    background: var(--teal);
  }

  .intro_container button:hover {
      background: transparent;
      color: var(--teal);
  }

  /* media ---------------- */
  @media (max-width: 1000px) {
      .intro_container p {
          font-size: 20px;
      }
  }
</style>