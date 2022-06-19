<template>
    <label class="option-checkbox">
        <input type="checkbox" name="password-length" id="">
        {{props.label}}
    </label>
</template>

<style scoped >
  .option-checkbox {
    display: flex;
    align-items: center;
    gap: 0.4em;
    color: #043730;
    font-size: 14px;
    font-weight: 500;
  }

  input[type="checkbox"] {
    zoom: 1.8;
  }
</style>

<script setup lang="ts">
    import { defineProps } from "vue";

    export interface IProps {
      label: string;
    }

    const props = defineProps<IProps>();
</script>

<script lang="ts">
  export default {};
</script>