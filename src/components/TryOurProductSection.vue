<script setup lang="ts">
import CallToActionButtons from "./CallToActionButtons.vue";
</script>

<template>
  <section class="try-product">
    <h1 class="try-product__title">Try CommuniTraders Now!</h1>
    <CallToActionButtons />
  </section>
</template>

<style scoped>
.try-product {
  background-color: var(--dark-blue-bg);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 6rem;
  padding: 5rem 0;
  color: var(--white);
}
.try-product__title {
  font-size: 2.2rem;
  font-weight: 800;
}
</style>
