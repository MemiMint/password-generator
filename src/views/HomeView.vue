<template>
  <main>
    <HomeNavbar />
    <Hero />
    <section class="tool-section">
      <h2 style="color: #043730;">...OR...</h2>
      <p style="margin-top: 20px;">You can use our quick tool to generate a password</p>
      <QuickTool />
    </section>
  </main>
  <Footer />
</template>

<style>
  body {
    background-color: #F0ECE6;
  }

  .tool-section {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin-bottom: 100px;
  }
</style>

<script setup lang="ts">
    import Hero from "@/components/Hero.vue";
    import HomeNavbar from '@/components/HomeNavbar.vue';
    import QuickTool from "@/components/QuickTool.vue";
    import Footer from "@/components/Footer.vue";
</script>
