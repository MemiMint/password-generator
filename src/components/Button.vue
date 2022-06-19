<template>
    <button 
      class="btn" 
      :class="props.color"
      @click="emits('onClick')"
    >
      {{props.label}}
    </button>
</template>

<style scoped>
  .btn {
    padding: 10px 40px 10px 40px;
    border: none;
    font-size: 15px;
    font-weight: 600;
    border-radius: 4px;
    cursor: pointer;
    transition: ease-in 0.3s;
  }

  .primary {
    background-color: #043730;
    color: white;
  }

  .secondary {
    color: white;
    background-color: #EE5B47;
  }

  .primary:hover {
    background-color: #1c4b44;
  }

  .secondary:hover {
    background-color: #b63221;
  }
</style>

<script setup lang="ts">
    import { defineProps, defineEmits } from 'vue';
    
    interface IProps {
      label: string;
      color: "primary" | "secondary"
    }

    interface IEmits {
      (e: string): void;
    }

    const props = defineProps<IProps>();
    const emits = defineEmits<IEmits>();
</script>

<script lang="ts">
export default {}
</script>
