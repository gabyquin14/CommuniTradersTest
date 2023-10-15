<script setup lang="ts">
import BenefitsListItems from "@/components/BenefitsListItems.vue";

const befenitsInfo = [
  {
    icon: "/src/assets/plant.svg",
    title: "Ideal for Beginner Clients",
    description:
      "Increase trading volumes as new traders gain comfort by following successful traders in forex markets and beyond into stocks, options, commodities, and more…",
  },
  {
    icon: "/src/assets/lock.svg",
    title: "Low Barriers to Entry",
    description:
      "CommuniTraders software is free and clients can start with just a $100 minimum investment.",
  },
  {
    icon: "/src/assets/magic-wand.svg",
    title: "Simple Interface",
    description:
      "A simple GUI provides needed features and tools but isn’t bogged down by non-core features. This allows clients to get setup quickly and start trading.",
  },
  {
    icon: "/src/assets/broken-link.svg",
    title: "No Long-Term Commitments",
    description:
      "Clients can easily signup to start, change signal providers, or stop the service. There is no long-term lockup.",
  },
  {
    icon: "/src/assets/security-shield.svg",
    title: "Funds Safety",
    description:
      "CommuniTraders benefits from the same strong regulation and banking partners standalone Tradeview clients enjoy along with transparency and negative balance protection.",
  },
  {
    icon: "/src/assets/certificate.svg",
    title: "Tradeview Runs CommuniTrader",
    description:
      "You will experience the Tradeview service you know and love, no gimmicks or hidden fees, excellent live customer support, and your dedicated account manager.",
  },
];
</script>

<template>
  <section class="benefits">
    <div class="benefits-list">
      <BenefitsListItems
        v-for="benefit in befenitsInfo"
        :icon="benefit.icon"
        :title="benefit.title"
        :description="benefit.description"
      />
    </div>
  </section>
</template>

<style scoped>
.benefits {
  width: 100%;
  background-color: var(--white);
}
.benefits-list {
  grid-gap: 30px;
  display: grid;
  grid-template-rows: repeat(auto, 1fr);
  padding: 5rem 0;
  width: 90%;
  margin: 0 auto;
}
@media screen and (min-width: 570px) {
  .benefits-list {
    padding: 10em 0;
    grid-template-columns: repeat(2, 1fr);
  }
}
@media screen and (min-width: 800px) {
  .benefits-list {
    grid-template-columns: repeat(3, 1fr);
  }
}
</style>
