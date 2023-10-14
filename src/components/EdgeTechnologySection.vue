<script setup lang="ts"></script>

<template>
  <section class="edge-tech">
    <div class="edge-tech__content">
      <div class="edge-tech__info">
        <h2 class="edge-tech__title">Leading Edge Technology</h2>
        <p class="edge-tech__description">
          Easy to use management tools, our fastest possible execution and
          spreads as low as 0.0.
        </p>
        <a class="edge-tech__link" href="" target="_blank"
          >Quick Guide: CommuniTraders Web User Manual
          <img src="@/assets/external-link.svg" alt=""
        /></a>
      </div>
      <img
        src="@/assets/trade-interface.png"
        alt="trade-interface"
        class="edge-tech__trade-interface"
      />
    </div>
  </section>
</template>

<style>
.edge-tech {
  color: var(--dark-text);
  background-color: var(--white);
}
.edge-tech__content {
  width: 90%;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 5rem;
}
.edge-tech__info {
  display: flex;
  align-items: flex-start;
  justify-content: center;
  flex-direction: column;
  gap: 1rem;
}
.edge-tech__title {
  font-size: 2.2rem;
}
.edge-tech__description {
  font-size: 1.5rem;
}
.edge-tech__link {
  font-size: 1.3rem;
  text-decoration: underline;
}
.edge-tech__link img {
  margin-left: 0.5rem;
}
.edge-tech__trade-interface {
  width: 80%;
}

@media screen and (min-width: 700px) {
  .edge-tech__content {
    flex-direction: row;
  }
  .edge-tech__trade-interface {
    width: 50%;
  }
}
</style>
