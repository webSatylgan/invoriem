<script setup>

</script>

<template>
  <div class="container">
    <div class="we">
      <h2>We are Invoriem</h2>
      <p>We fulfill international property developments</p>
      <div class="we_video">
        <img src="" alt="">
        <svg class="we-video_play" width="120" height="120" viewBox="0 0 120 120" fill="none" xmlns="http://www.w3.org/2000/svg">
          <circle cx="60" cy="60" r="60" fill="black" fill-opacity="0.7" />
          <circle cx="60" cy="60" r="59" stroke="white" stroke-opacity="0.5" stroke-width="2" />
          <path d="M47 78.1149V42.6235C47 41.0494 48.7341 40.0923 50.0659 40.9312L76.4782 57.5678C77.6814 58.3257 77.7316 60.0617 76.5743 60.8879L50.162 79.7427C48.8382 80.6877 47 79.7414 47 78.1149Z" fill="white" />
        </svg>
      </div>
    </div> <!-- we -->
  </div>
</template>

<style scoped>
  .we {
    width: 100%;
    margin-top: 300px;
  }

  .we p {
    margin-top: 50px;
  }

  .we_video {
    width: 100%;
    height: 1000px;
    margin-top: 80px;

    background: url("@assets/imgs/Video.png") center/cover no-repeat;

    position: relative;
  }

  .we_video svg {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

</style>