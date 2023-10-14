<script setup lang="ts">
interface Props {
  icon: string;
  title: string;
  description: string;
}

const { icon, title, description } = defineProps<Props>();
</script>

<template>
  <article class="benefit-card">
    <div class="benefit-card__content">
      <img :src="icon" alt="benefit-icon" class="benefit-card__icon" />
      <h3 class="benefit-card__title">
        {{ title }}
      </h3>
      <p class="benefit-card__description">{{ description }}</p>
    </div>
  </article>
</template>

<style scoped>
.benefit-card {
  background-color: var(--white);
  box-shadow: 0 0 30px rgba(0, 0, 0, 0.078) !important;
  height: 100%;
  width: auto;
  display: flex;
  flex-direction: column;
  font-size: 1.3rem;
}
.benefit-card__icon {
  height: 3.2rem;
  width: auto;
  object-fit: contain;
}
.benefit-card__content {
  background: var(--white);
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
  text-align: left;
  padding: 2rem;
  transition: 0.2s ease;
  gap: 1rem;
}

.benefit-card__title {
  color: var(--accent-red);
}

.benefit-card__description {
  color: var(--dark-text);
}
</style>
