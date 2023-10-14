<script setup lang="ts">
import Header from "@/components/TheHeader.vue";
import Footer from "@/components/TheFooter.vue";
</script>

<template>
  <Header />
  <div class="main-layout">
    <slot />
  </div>
  <Footer />
</template>

<style>
.main-layout {
  /* margin: 0 auto;
  max-width: 90%; */
}
</style>
