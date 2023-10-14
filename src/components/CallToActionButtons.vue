<script setup lang="ts">
import AppMainButton from "./AppMainButton.vue";
</script>

<template>
  <section class="call-to-action">
    <div class="call-to-action__options">
      <h3 class="call-to-action__subtitle">
        Free Download for Tradeview Users
      </h3>
      <AppMainButton text="Contact your Broker" type="outlined" />
    </div>
    <div class="separator"></div>
    <div class="call-to-action__options">
      <h3 class="call-to-action__subtitle">
        Free Download for Tradeview Users
      </h3>
      <AppMainButton text="Get a Free Demo" type="filled" />
    </div>
  </section>
</template>

<style scoped>
.call-to-action {
  display: flex;
  flex-direction: column;
  gap: 2.5rem;
}

.call-to-action__options {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2rem;
  max-width: 17rem;
}
.call-to-action__subtitle {
  font-weight: 400;
  text-align: center;
}
</style>
