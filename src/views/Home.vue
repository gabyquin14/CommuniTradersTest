<script setup lang="ts">
import BenefitsList from "@/components/BenefitsListSection.vue";
import EdgeTechnology from "@/components/EdgeTechnologySection.vue";
import TryOurProduct from "../components/TryOurProductSection.vue";
import HeroPresentation from "../components/HeroPresentationSection.vue";
import MainLayout from "@/layouts/MainLayout.vue";
</script>

<template>
  <MainLayout class="parallax-container">
    <div class="parallax-background">
      <HeroPresentation />
    </div>
    <div class="parallax-foreground">
      <BenefitsList />
      <EdgeTechnology />
      <TryOurProduct />
    </div>
  </MainLayout>
</template>

<style scoped>
@media screen and (min-width: 850px) {
  .parallax-container {
    position: relative;
    overflow: hidden;
  }

  .parallax-background {
    top: 8rem;
    width: 100%;
    position: sticky;
    z-index: 1;
  }

  .parallax-foreground {
    position: relative;
    z-index: 2;
  }
}
</style>
