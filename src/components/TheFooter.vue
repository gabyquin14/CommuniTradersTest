<script setup lang="ts">
import FooterLegalDeclarations from "@/components/FooterLegalDeclarations.vue";
import AppMainButton from "@/components/AppMainButton.vue";
</script>

<template>
  <footer class="footer">
    <div class="footer__content">
      <section class="footer__main-info">
        <img
          class="footer__communi-logo"
          src="https://www.tvmarkets.com/_nuxt/img/logo_white.0f9805e.svg"
          alt="Communi-traders"
        />
        <nav class="footer__find-us separator-border">
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
                  src="../assets/facebook.png"
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
        <div class="footer__subscribe-newsletter separator-border">
          <div class="footer__newsletter-slogan">
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
          <div class="footer__newsletter-input__container">
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
        <div class="footer__nav-container">
          <nav class="main-nav separator-border">
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
          <div class="secondary-nav separator-border">
            <div class="secondary-navflex-col">
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
            <div>
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
.separator-border {
  padding: 2rem 0;
  border-bottom: solid 0.1rem var(--border-separator);
}
.footer {
  background-color: var(--dark-gray-bg);
  color: var(--light-text);
  box-shadow: inset 1px 38px 34px -24px rgba(0, 0, 0, 0.65);
}
.footer__content {
  width: 90%;
  margin: 0 auto;
  padding: 5rem 0;
}
.footer__actions-container {
  margin-bottom: 2rem;
}
.footer__main-info {
  display: flex;
  flex-direction: column;
}
.footer__communi-logo {
  width: 70%;
  margin: 0 auto 4rem;
}
.footer__find-us {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1.5rem;
}
.footer__find-us__subtitle {
  font-weight: 300;
}
.footer__find-us__navigation {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1rem;
}
.footer__navigation__img {
  object-fit: contain;
  width: 2rem;
  height: 2rem;
}
.footer__tradeview-markets p {
  width: 80%;
  margin: 0 auto;
}
/*NEWSLETTER STYLES */
.footer__subscribe-newsletter {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.footer__newsletter-slogan {
  display: flex;
  flex-direction: column;
}
.footer__surfs-up {
  width: 60%;
  margin: 2rem auto;
}
.footer__newsletter-slogan p {
  width: 90%;
  margin: 0 auto;
  text-align: center;
}
.footer__newsletter-input__container {
  width: 80%;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
  margin: 0 auto 2rem;
}
.footer__newsletter-input__container .main-button,
.footer__newsletter__input {
  width: 100%;
}
.footer__newsletter__input {
  height: 4.7rem;
  background-color: transparent;
  border: solid 0.1rem var(--border-separator);
  outline: none;
  box-sizing: border-box;
}
.footer__newsletter__input[type="text"] {
  padding-left: 1rem;
}
/*NAVIGATIONS STYLES */
.main-nav {
  width: 90%;
  margin: 0 auto;
  padding: 4rem 0;
}
.main-nav__list {
  text-decoration: underline;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2.5rem;
  font-size: 1.3rem;
  letter-spacing: 0.2rem;
}
.secondary-nav {
  display: grid;
  grid-template-columns: 1fr 1fr;
  padding: 2rem 0;
}
.secondary-nav__nav-links {
  gap: 1rem;
  margin-top: 2rem;
}
.secondary-nav__nav-links ul {
  gap: 0.5rem;
  font-size: 1.3rem;
}
@media screen and (min-width: 800px) {
  .footer__content {
    display: flex;
    justify-content: space-between;
    font-size: 1.3rem;
    width: 90%;
  }
  .footer__communi-logo {
    width: 60%;
    margin: 0 0 2rem;
  }
  .footer__subscribe-newsletter {
    display: flex;
    flex-direction: column;
    gap: 2rem;
    border: solid 0.1rem var(--dark-gray-footer);
    padding: 2rem;
    max-width: 70rem;
  }
  .footer__newsletter-slogan {
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    gap: 2rem;
  }
  .vertical-separator {
    display: block;
    width: 0.1rem;
    height: 5rem;
    background-color: var(--white);
  }
  .footer__surfs-up {
    max-width: 16rem;
    margin: 0;
  }
  .footer__newsletter-slogan p {
    width: 60%;
    margin: 0;
  }
  .footer__newsletter-input__container {
    width: 100%;
    flex-direction: row;
  }
  .footer__newsletter-input__container .main-button {
    width: 17rem;
  }
  .footer__find-us {
    order: 3;
    border: none;
    padding: 2rem 0 0;
    align-items: flex-start;
  }

  .footer__tradeview-markets {
    order: 2;
    border: none;
    padding: 0;
  }
  .footer__tradeview-markets p {
    margin: 0;
  }
  .footer__main-info {
    gap: 2rem;
  }
  .main-nav {
    width: fit-content;
    padding: 4rem 4rem 0 0;
    border: none;
    margin: 0;
  }
  .secondary-nav {
    width: fit-content;
    gap: 4rem;
    border: none;
    margin: 0;
  }
  .main-nav__list {
    width: fit-content;
    align-items: flex-start;
  }
  .footer__nav-container {
    display: flex;
  }
}
@media screen and (min-width: 1100px) {
  .footer__content {
    width: 70%;
  }
}
</style>
