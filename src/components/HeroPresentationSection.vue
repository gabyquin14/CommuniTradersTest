<script setup lang="ts">
import CallToActionButtons from "./CallToActionButtons.vue";
</script>

<template>
  <section class="hero">
    <div class="hero__body">
      <div class="hero__devices">
        <img
          src="https://www.tvmarkets.com/_nuxt/img/LAPTOP-PHONE-5.51ab6a1.png"
          class="hero__communi-traders-devices"
          alt="communi-traders-logo"
        />
      </div>

      <div class="hero__content">
        <img
          src="https://www.tvmarkets.com/_nuxt/img/logo1.caa2e62.svg"
          class="hero__communi-logo"
          alt=""
        />
        <hr class="separator" />
        <p class="hero__description">
          Tradeview’s <b>CommuniTraders</b> software lets our partners provide
          value-added copy trading to their clients.
        </p>
        <CallToActionButtons style="gap: 4rem" />
      </div>
    </div>
  </section>
</template>

<style scoped>
.hero {
  background-color: var(--dark-blue-bg);
  color: var(--white);
}
.hero__devices {
  width: 100%;
  background-color: #d2d8dc;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 2rem 0;
}
.hero__body {
  display: flex;
  flex-direction: column-reverse;
  height: 100%;
}
.hero__communi-logo {
  width: 60%;
  margin-bottom: 2rem;
}
.hero__communi-traders-devices {
  width: 70%;
  object-fit: contain;
}
.hero__content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 2rem;
  width: 90%;
  margin: 6rem auto;
}
.separator {
  height: 0.1rem;
  width: 80%;
  background-color: var(--white);
}
.hero__description {
  font-size: 2rem;
  text-align: center;
  margin-bottom: 4rem;
  font-weight: 300;
}
@media screen and (min-width: 580px) {
  .hero__body {
    flex-direction: row;
  }
  .hero__communi-logo {
    width: 50%;
  }
  .hero__devices {
    width: 75%;
  }
  .hero__description {
    width: 90%;
  }
}
@media screen and (min-width: 1000px) {
  .hero {
    height: calc(100vh - 5rem);
  }
  .hero__content {
    width: 90%;
  }
  .hero__communi-logo {
    width: 45%;
    margin-bottom: 4rem;
  }
  .hero__communi-traders-devices {
    width: 70%;
    object-fit: contain;
  }
  .hero__description,
  .separator {
    width: 60%;
  }
  .hero__devices {
    width: 80%;
  }
}
</style>
