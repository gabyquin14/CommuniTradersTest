<script setup lang="ts">
interface Props {
  text: string;
  type: "outlined" | "filled";
  activeColor?: string;
}

const { text, type, activeColor } = defineProps<Props>();
</script>

<template>
  <button
    class="main-button"
    :class="type"
    :style="{
      backgroundColor: activeColor,
      border: 'solid 0.1rem' + activeColor,
    }"
  >
    {{ text }}
  </button>
</template>

<style scoped>
.main-button {
  font-size: 1.3rem;
  font-weight: 600;
  outline: none;
  text-align: center;
  transition: 0.3s;
  height: 47px;
  width: 170px;
}
.filled {
  border: solid 0.1rem var(--accent-red);
  background-color: var(--accent-red);
  color: var(--white);
}

.outlined {
  border: solid 0.1rem var(--white);
  background-color: transparent;
  color: var(--white);
}
</style>
