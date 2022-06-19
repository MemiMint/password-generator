<template>
    <footer>
        <Logo bg="white" color="white" />
        <p class="copyright">&copy; Copyright {{ year }} by <a href="" style="text-decoration: none; color: #EE5B47;">Memi.</a></p>
    </footer>
</template>

<style scoped>
  footer {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    padding: 20px;
    height: 20vh;
    background-color: #043730;
  }

  .copyright {
    color: white;
    font-weight: 500;
    margin-top: 40px;
  }
</style>

<script setup lang="ts">
    import { ref } from "vue";
    import Logo from "@/components/Logo.vue";

    const year = ref<string>(new Date().getFullYear().toString())
</script>

<script lang="ts" > 
    export default {};
</script>
