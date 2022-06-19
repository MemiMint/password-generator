<template>
    <div class="tool">
        <div class="tool-options-container">
            <Checkbox v-for="label in checkboxes" :key="label" :label="label" />
            <LengthInput label="Password Length" />
        </div>
        <div v-if="show" class="password-text">
            <div class="password" >
              <p>wGeWqGiFmQtWxZlUyOrZ</p>
            </div>
            <p id="copy">copy</p>
        </div>
        <div class="tool-btn-container">
            <Button @onClick="toggleShow()" color="primary" label="Generate Password" />
        </div>
    </div>
</template>

<style scoped>
  .tool {
    margin-top: 40px;
    background-color: #c5bcb1;
    padding: 20px;
    border-radius: 10px;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .tool-options-container {
    display: flex;
    align-items: center;
    gap: 1em;
  }

  .password-text {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px 20px 10px 20px;
    background-color: #F0ECE6;
    color: #6c707b;
    border-radius: 10px;
    margin-top: 40px;
    font-size: 18px;
  }

  .password-text #copy {
    font-size: 14px;
    font-weight: 500;
    cursor: pointer;
  }

  .password-text #copy:hover {
    font-weight: 600;
  }

  .password {
    flex: 1;
    text-align: center;
  }

  .tool-btn-container {
    margin-top: 40px;
    display: flex;
    align-items: center;
    justify-content: center;
  }
</style>

<script setup lang="ts">
    import { ref } from "vue";
    import Checkbox from "@/components/Checkbox.vue";
    import LengthInput from "@/components/LengthInput.vue";
    import Button from "@/components/Button.vue";

    const show = ref<boolean>(false);

    const checkboxes = ref<string[]>([
        "Include uppercase letters",
        "Include lowercase letters",
        "Include numbers",
        "Include symbols"
    ]);

    const toggleShow = () => {
        show.value = !show.value;
    }
</script>

<script lang="ts">
  export default {};
</script>