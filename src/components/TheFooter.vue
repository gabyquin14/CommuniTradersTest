<script setup lang="ts">
import FooterLegalDeclarations from "@/components/FooterLegalDeclarations.vue";
import AppMainButton from "@/components/AppMainButton.vue";
</script>

<template>
  <footer class="footer">
    <div class="footer__content">
      <section class="footer__main-info flex-col">
        <img
          class="footer__communi-logo"
          src="https://www.tvmarkets.com/_nuxt/img/logo_white.0f9805e.svg"
          alt="Communi-traders"
        />
        <nav class="footer__find-us flex-col separator-border vertical-padding">
          <h3 class="footer__find-us__subtitle">Find us on:</h3>
          <ul class="footer__find-us__navigation">
            <li>
              <a href=""
                ><img
                  class="footer__navigation__img"
                  src="https://www.tvmarkets.com/_nuxt/img/icon_twitter.f5da6c2.svg"
                  alt="Twitter"
              /></a>
            </li>
            <li>
              <a href=""
                ><img
                  class="footer__navigation__img"
                  src="../assets/images/facebook.png"
                  alt="Facebook"
              /></a>
            </li>
            <li>
              <a href=""
                ><img
                  class="footer__navigation__img"
                  src="https://www.tvmarkets.com/_nuxt/img/icon_linkedin.54df89e.svg"
                  alt="Linkedin"
              /></a>
            </li>
            <li>
              <a href=""
                ><img
                  class="footer__navigation__img"
                  src="https://tvmarkets.com/_nuxt/img/icon_instagram.3be0c20.svg"
                  alt="Instagram"
              /></a>
            </li>
            <li>
              <a href=""
                ><img
                  class="footer__navigation__img"
                  src="https://www.tvmarkets.com/_nuxt/img/icon_youtube.d7756da.svg"
                  alt="Youtube"
              /></a>
            </li>
          </ul>
        </nav>
        <div class="footer__tradeview-markets separator-border">
          <p>
            <b>Tradeview Markets</b> | Grand Cayman, KY1-1002, 4th Floor Harbour
            Place | 103 South Church St, PO Box 1105
            <br />
            <b>Main Oﬃce:</b> +1 345 945 6271
            <br />
            <b>Direct Phone:</b> +1 345 946 4532
            <br />
            <b>Website:</b> www.tvmarkets.com
          </p>
        </div>
      </section>
      <section class="footer__actions-container">
        <div
          class="footer__subscribe-newsletter flex-col separator-border vertical-padding"
        >
          <div class="footer__newsletter-slogan flex-col">
            <img
              class="footer__surfs-up"
              src="https://www.tvmarkets.com/_nuxt/img/surfs-up-gray.e67323f.svg"
              alt="Surfs up"
            />
            <div class="vertical-separator"></div>
            <p>
              Find daily trading insights and understand what is behind the
              latest waves in financial markets.
            </p>
          </div>
          <div class="footer__newsletter-input__container flex-col">
            <input
              class="footer__newsletter__input"
              type="text"
              placeholder="Enter your email address"
            />
            <AppMainButton
              text="Subscribe"
              type="filled"
              activeColor="#4B4D5C"
            />
          </div>
        </div>
        <div class="footer__nav-container separator-border">
          <nav class="main-nav separator-border vertical-padding">
            <ul class="main-nav__list">
              <li><a href="">FOREX</a></li>
              <li><a href="">STOCKS</a></li>
              <li><a href="">FUTURES</a></li>
              <li><a href="">TradeGATEHub</a></li>
              <li><a href="">MARKETS</a></li>
              <li><a href="">PRICING</a></li>
              <li><a href="">INTRODUCING BROKERS</a></li>
              <li><a href="">EDUCATION</a></li>
              <li><a href="">CONTACT US</a></li>
            </ul>
          </nav>
          <div class="secondary-nav separator-border vertical-padding">
            <div class="secondary-nav__container flex-col">
              <nav class="secondary-nav__nav-links flex-col">
                <h3 class="secondary-nav__nav-subtitle">ACCOUNTS</h3>
                <ul class="flex-col">
                  <li><a href="">Open account</a></li>
                  <li><a href="">Individual</a></li>
                  <li><a href="">Joint</a></li>
                  <li><a href="">Corporate</a></li>
                </ul>
              </nav>
              <nav class="secondary-nav__nav-links flex-col">
                <h3 class="secondary-nav__nav-subtitle">ABOUT TRADEVIEW</h3>
                <ul class="flex-col">
                  <li><a href="">Our Story</a></li>
                  <li><a href="">Our Team</a></li>
                  <li><a href="">Our Vision</a></li>
                </ul>
              </nav>
              <nav class="secondary-nav__nav-links flex-col">
                <h3 class="secondary-nav__nav-subtitle">COMPANY</h3>
                <ul class="flex-col">
                  <li><a href="">Why Tradeview</a></li>
                  <li><a href="">Sponsorships</a></li>
                  <li><a href="">Press</a></li>
                </ul>
              </nav>
            </div>
            <div class="secondary-nav__container flex-col">
              <nav class="secondary-nav__nav-links flex-col">
                <h3
                  class="secondary-nav__nav-subtitle"
                  style="text-decoration: underline"
                >
                  SOFTWARE
                </h3>
                <ul class="flex-col">
                  <li><a href="">MetaTrader 4</a></li>
                  <li><a href="">MetaTrader 5</a></li>
                  <li><a href="">cTrader</a></li>
                  <li><a href="">cTrader Copy</a></li>
                  <li><a href="">CurreneX</a></li>
                </ul>
              </nav>
              <nav class="secondary-nav__nav-links flex-col">
                <h3 class="secondary-nav__nav-subtitle">SUPPORT</h3>
                <ul class="flex-col">
                  <li><a href=""> Forms and Documents </a></li>
                  <li><a href="">FAQ</a></li>
                </ul>
              </nav>
            </div>
          </div>
        </div>
      </section>
    </div>
    <FooterLegalDeclarations />
  </footer>
</template>

<style scoped>
@import url("../assets/css/footer.css");
</style>
