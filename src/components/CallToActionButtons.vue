<script setup lang="ts">
import AppMainButton from "./AppMainButton.vue";
</script>

<template>
  <section class="call-to-action flex-col">
    <div class="call-to-action__options flex-col">
      <h3 class="call-to-action__subtitle">
        Free Download for Tradeview Users
      </h3>
      <AppMainButton text="Contact your Broker" type="outlined" />
    </div>
    <div class="separator"></div>
    <div class="call-to-action__options flex-col">
      <h3 class="call-to-action__subtitle">
        Free Download for Tradeview Users
      </h3>
      <AppMainButton text="Get a Free Demo" type="filled" />
    </div>
  </section>
</template>

<style scoped>
.call-to-action {
  gap: 2rem;
}

.call-to-action__options {
  align-items: center;
  gap: 2rem;
  max-width: 17rem;
}
.call-to-action__subtitle {
  font-size: 1.3rem;
  font-weight: 300;
  text-align: center;
}

@media screen and (min-width: 820px) {
  .call-to-action {
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 4rem;
    height: 14rem;
  }
  .separator {
    height: 100%;
    width: 0.1rem;
    min-width: 0.1rem;
    background-color: var(--white);
  }
  .call-to-action__options {
    max-width: unset;
  }
}
@media screen and (min-width: 1000px) {
  .call-to-action {
    gap: 10rem;
  }
}
</style>
