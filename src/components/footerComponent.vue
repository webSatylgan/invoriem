<script setup>

</script>

<template>
  <div class="container">
    <div class="footer flex">
      <p>Copyright © 2020 Invoriem</p>
      <div class="footer_info flex">
        <p>info@invoriem.com</p>
        <div class="footer_social flex">
          <a href=""><img src="@assets/imgs/instagram.svg" alt=""></a>
          <a href=""><img src="@assets/imgs/facebook.svg" alt=""></a>
          <a href=""><img src="@assets/imgs/twitter.svg" alt=""></a>
          <a href=""><img src="@assets/imgs/linkedIn.svg" alt=""></a>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
  .footer{
    margin-top: 200px;
  }

  .footer p {
    font-size: 20px;
  }

  .footer_info {
    max-width: 530px;
  }

  .footer_social {
    max-width: 240px;
  }

  @media (max-width: 600px) {
      .footer {
          flex-direction: column;
          gap: 30px;
      }
  }

  @media (max-width: 520px) {
      .footer_info {
          flex-direction: column;
          gap: 15px;
      }
  }
</style>