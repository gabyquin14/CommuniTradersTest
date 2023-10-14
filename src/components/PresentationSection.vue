<script setup lang="ts">
import CallToActionButtons from "./CallToActionButtons.vue";
</script>

<template>
  <section class="hero">
    <div class="hero-content">
      <img src="@/assets/hero.png" alt="" />
      <div>
        <img src="@/assets/communi-traders-white.svg" alt="" />
        <div class="separator"></div>
        <p>
          Tradeview’s CommuniTraders software <br />lets our partners provide
          value-added copy <br />trading to their clients.
        </p>
        <CallToActionButtons />
      </div>
    </div>
  </section>
</template>

<style scoped>
.hero {
  display: flex;
  flex-direction: column-reverse;
  background-color: var(--dark-blue-bg);
}
</style>
