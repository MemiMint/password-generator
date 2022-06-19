<template>
    <header>
        <Logo bg="#043730" color="#043730" />
        <nav class="nav" >
            <ul>
                <li>
                    <a href="">Github</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style scoped>
    header {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 20px;
    }

    .nav ul {
        list-style: none;
    }

    .nav a {
        text-decoration: none;
        color: #043730;
        font-weight: 500;
        font-size: 15px;
    }
</style>

<script setup lang="ts">
    import Logo from './Logo.vue';
</script>

<script lang="ts">
export default {};
</script>