<script setup>

</script>

<template>
  <button>
    <slot></slot>
    <svg width="28" height="16" viewBox="0 0 28 16" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M20.6863 0L19.4657 1.47037C19.4657 1.47037 22.6405 4.76444 24.8317 6.82296C17.1461 6.74074 0 6.8237 0 6.8237V8.58815C0 8.58815 17.1518 8.5237 24.8346 8.58815C22.6434 10.9407 19.4686 14.2356 19.4686 14.2356L20.6863 16L28 7.7037L20.6863 0Z" />
    </svg>
  </button>
</template>

<style scoped>
  button {
    display: flex;
    align-items: center;
    padding: 10px 25px;
    border: 1px solid var(--teal);
  }

  button svg {
    margin-left: 15px;

    fill: currentColor;
    transition: .2s;
  }
  /* button hover animation */
  button:hover {
    color: #fff;
    background: var(--teal);
  }
</style>