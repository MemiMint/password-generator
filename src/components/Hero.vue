<template>
  <section class="hero">
    <h1>Password Generator</h1>
    <p>Generate and manage your password to your accounts in a easy way</p>
    <div class="btn-container" >
      <Button label="Sign In" color="primary" />
      <Button label="Create Account" color="secondary" />
    </div>
  </section>
</template>

<style scoped>
  .hero {
    display: flex;
    align-items: center;
    flex-direction: column;
    justify-content: center;
    height: 40vh;
    padding: 10px 40px 10px 40px;
  }

  .hero h1 {
    font-size: 3.5em;
    color: #043730;
    font-weight: 500;
  }

  .hero p {
    font-size: 20px;
    font-weight: 400;
    color: #3c6761;
  }

  .btn-container {
    display: flex;
    align-items: center;
    margin-top: 40px;
    gap: 1.5em;
  }
</style>

<script setup lang="ts">
  import Button from './Button.vue';
</script>

<script lang="ts">
  export default {};
</script>
