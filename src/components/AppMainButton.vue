<script setup lang="ts">
import { computed } from "vue";

interface Props {
  text: string;
  type: "outlined" | "filled";
  activeColor?: string;
}

const { text, type, activeColor } = defineProps<Props>();

const styleObject = computed(() => {
  return {
    "--color": activeColor || "var(--accent-red)",
    "--color-hover": activeColor ? activeColor + "aa" : "#ff0000ed",
  };
});
</script>

<template>
  <button class="main-button" :class="type" :style="styleObject">
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
  z-index: 2;
}
.filled {
  border: solid 0.1rem var(--color);
  background-color: var(--color);
  color: var(--white);
}

.outlined {
  border: solid 0.1rem var(--white);
  background-color: transparent;
  color: var(--white);
}
.filled:hover {
  background-color: var(--color-hover);
  border: solid 0.1rem var(--color-hover);
}

.outlined:hover {
  background-color: rgba(255, 255, 255, 0.119);
}
</style>
