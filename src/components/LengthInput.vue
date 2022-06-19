<template>
    <label class="password-length" for="max-length">
        {{props.label}}
        <input min="0" type="number" name="max-length" id="">
    </label>
</template>

<style scoped>
    .password-length {
        color: #043730;
        gap: 1.5em;
        font-size: 14px;
        font-weight: 500;
    }

    input[type="number"] {
        width: 60px;
        height: 40px;
        padding: 10px;
        font-family: 'Poppins';
        font-weight: 500;
        border-radius: 4px;
        border: 2px solid rgba(0, 0, 0, 0.8);
        color: #6c707b;
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