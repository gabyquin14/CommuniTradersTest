<script setup lang="ts">
import BenefitsList from "@/components/BenefitsListSection.vue";
import EdgeTechnology from "@/components/EdgeTechnologySection.vue";
import TryOurProduct from "../components/TryOurProductSection.vue";
import Presentation from "../components/PresentationSection.vue";
import MainLayout from "@/layouts/MainLayout.vue";
</script>

<template>
  <MainLayout>
    <Presentation />
    <BenefitsList />
    <EdgeTechnology />
    <TryOurProduct />
  </MainLayout>
</template>

<style scoped></style>
