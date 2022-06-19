<template>
    <div :style="{color: props.color}" class="logo">
        <div :style="{backgroundColor: props.bg}" class="logo-bg">
            <img src="@/assets/icons8-contraseña-1-48.png" alt="" srcset="">
        </div>
        <p>Password Generator</p>
    </div>
</template>

<style scoped>
    .logo {
        display: flex;
        align-items: center;
        gap: 1em;
        font-size: 16px;
    }
    .logo-bg {
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 10px;
        border-radius: 100%;
    }

    .logo-bg img {
        width: 28px;
        height: 28px;
    }
</style>

<script setup lang="ts">
    import { defineProps } from "vue";

    interface IProps {
        color: string;
        bg: string;
    }

    const props = defineProps<IProps>();
</script>

<script lang="ts">
export default {};
</script>

