<script setup lang="ts">
import ExternalLink from "@/assets/images/external-link.vue";
import { ref } from "vue";

const showMenu = ref(false);
</script>

<template>
  <header class="header">
    <div class="header__container">
      <a
        href="/"
        class="header__logo"
        style="flex: 1"
        aria-label="Tradeview Home"
      >
        <img
          src="https://www.tvmarkets.com/_nuxt/img/logo_tradeview_full_dark.4bc1faa.svg"
          alt="Tradeview Logo"
        />
      </a>
      <nav class="header__primary-nav header__main-nav">
        <ul>
          <li><a href="/forex">Forex</a></li>
          <li><a href="/stocks">Stocks</a></li>
          <li><a href="/futures">Futures</a></li>
          <li><a href="/tradegatehub">TradeGATEHub</a></li>
        </ul>
      </nav>
      <nav class="header__primary-nav" style="flex: 1">
        <ul>
          <li><a href="/login">Login</a></li>
          <li>|</li>
          <li><a href="/contact">Contact us</a></li>
          <li class="header__primary-nav__language-link">
            English
            <img src="@/assets/images/world-language.svg" alt="Language" />
            <img src="@/assets/images/chevron-down.svg" alt="Dropdown" />
          </li>
        </ul>
      </nav>
      <button
        class="header__hamburger-menu"
        @click="showMenu = !showMenu"
        role="button"
        :aria-expanded="showMenu"
        aria-label="Toggle Menu"
      >
        <span class="line top-line" aria-hidden="true"></span>
        <span class="line middle-line" aria-hidden="true"></span>
        <span class="line bottom-line" aria-hidden="true"></span>
      </button>
    </div>
    <nav
      class="header__second-nav__container flex-col"
      :class="showMenu ? 'show-menu' : ''"
    >
      <span class="header__second-nav__extra-items">
        <a href="/login">Login</a>
        <ExternalLink color="var(--white)" style="margin-left: auto" />
      </span>
      <nav class="header__second-nav__content">
        <ul class="flex-col">
          <li class="header__second-nav__nav-link">
            <a href="/markets">Markets</a>
          </li>
          <li class="header__second-nav__nav-link">
            <a href="/company"
              >Company
              <img src="@/assets/images/chevron-down.svg" alt="Dropdown" />
            </a>
          </li>
          <li class="header__second-nav__nav-link">
            <a href="/accounts">Accounts</a>
          </li>
          <li class="header__second-nav__nav-link">
            <a href="/platforms"
              >Platforms
              <img src="@/assets/images/chevron-down.svg" alt="Dropdown" />
            </a>
          </li>
          <li class="header__second-nav__nav-link">
            <a href="/pricing">Pricing</a>
          </li>
          <li class="header__second-nav__nav-link">
            <a href="/brokers">Introducing brokers</a>
          </li>
          <li class="header__second-nav__nav-link">
            <a href="/education">Education</a>
          </li>
          <li class="header__second-nav__nav-link">
            <a href="/support"
              >Support
              <img src="@/assets/images/chevron-down.svg" alt="Dropdown" />
            </a>
          </li>
        </ul>
      </nav>
      <span class="header__second-nav__extra-items extra-items__border">
        <b>TradeGATEHub</b>
      </span>
      <a href="/contact" class="header__second-nav__extra-items">Contact Us</a>
      <span class="header__second-nav__extra-items">
        <img src="@/assets/images/world-language.svg" alt="Language" />
        English
        <img
          style="margin-left: auto"
          src="@/assets/images/chevron-down.svg"
          alt="Dropdown"
        />
      </span>
    </nav>
  </header>
</template>

<style scoped>
@import url("../assets/css/header.css");
</style>
