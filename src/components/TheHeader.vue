<script setup lang="ts">
import ExternalLink from "@/assets/images/external-link.vue";
import { ref } from "vue";

const showMenu = ref(false);
</script>

<template>
  <header class="header">
    <div class="header__container">
      <img
        class="header__logo"
        style="flex: 1"
        src="https://www.tvmarkets.com/_nuxt/img/logo_tradeview_full_dark.4bc1faa.svg"
        alt=""
      />
      <nav class="header__first-content-nav header__main-nav">
        <ul>
          <li><a href="">Forex</a></li>
          <li><a href="">Stocks</a></li>
          <li><a href="">Futures</a></li>
          <li><a href="">TradeGATEHub</a></li>
        </ul>
      </nav>
      <nav class="header__first-content-nav" style="flex: 1">
        <ul>
          <li><a href="">Login</a></li>
          <li>|</li>
          <li><a href="">Contact us</a></li>
          <li class="header__first-content-nav__link">
            English <img src="@/assets/images/world-language.svg" alt="" />
            <img src="@/assets/images/chevron-down.svg" alt="" />
          </li>
        </ul>
      </nav>
      <button
        class="header__hamburger-menu"
        @click="showMenu = !showMenu"
        role="button"
        :aria-expanded="showMenu"
      >
        <span class="line top-line"></span>
        <span class="line middle-line"></span>
        <span class="line bottom-line"></span>
      </button>
    </div>
    <div
      class="header__second-nav__container flex-col"
      :class="showMenu ? 'show-menu' : ''"
    >
      <span class="header__second-nav__extra-items">
        Login <ExternalLink color="var(--white)" style="margin-left: auto" />
      </span>
      <nav class="header__second-nav__content">
        <ul class="flex-col">
          <li class="header__second-nav__nav-link"><a href="">Markets</a></li>
          <li class="header__second-nav__nav-link">
            <a href=""
              >Company <img src="@/assets/images/chevron-down.svg" alt=""
            /></a>
          </li>
          <li class="header__second-nav__nav-link"><a href="">Accounts</a></li>
          <li class="header__second-nav__nav-link">
            <a href=""
              >Platforms <img src="@/assets/images/chevron-down.svg" alt=""
            /></a>
          </li>
          <li class="header__second-nav__nav-link"><a href="">Pricing</a></li>
          <li class="header__second-nav__nav-link">
            <a href="">Introducing brokers</a>
          </li>
          <li class="header__second-nav__nav-link"><a href="">Education</a></li>
          <li class="header__second-nav__nav-link">
            <a href=""
              >Support <img src="@/assets/images/chevron-down.svg" alt=""
            /></a>
          </li>
        </ul>
      </nav>
      <span class="header__second-nav__extra-items extra-items__border"
        ><b>TradeGATEHub</b></span
      >
      <span class="header__second-nav__extra-items">Contact Us</span>
      <span class="header__second-nav__extra-items">
        <img src="@/assets/images/world-language.svg" alt="" />
        English
        <img
          style="margin-left: auto"
          src="@/assets/images/chevron-down.svg"
          alt="arrow-down"
        />
      </span>
    </div>
  </header>
</template>

<style scoped>
@import url("../assets/css/header.css");
</style>
