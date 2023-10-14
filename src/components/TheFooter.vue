<script setup lang="ts">
import FooterLegalDeclarations from "@/components/FooterLegalDeclarations.vue";
import AppMainButton from "@/components/AppMainButton.vue";
</script>

<template>
  <footer class="footer">
    <section>
      <img
        src="https://www.tvmarkets.com/_nuxt/img/logo_white.0f9805e.svg"
        alt=""
      />
      <nav class="footer__find-us">
        <ul>
          <li>
            <a href=""
              ><img
                src="https://www.tvmarkets.com/_nuxt/img/icon_twitter.f5da6c2.svg"
                alt=""
            /></a>
          </li>
          <li>
            <a href=""><img src="../assets/facebook.png" alt="" /></a>
          </li>
          <li>
            <a href=""
              ><img
                src="https://www.tvmarkets.com/_nuxt/img/icon_linkedin.54df89e.svg"
                alt=""
            /></a>
          </li>
          <li>
            <a href=""
              ><img
                src="https://tvmarkets.com/_nuxt/img/icon_instagram.3be0c20.svg"
                alt=""
            /></a>
          </li>
          <li>
            <a href=""
              ><img
                src="https://www.tvmarkets.com/_nuxt/img/icon_youtube.d7756da.svg"
                alt=""
            /></a>
          </li>
        </ul>
      </nav>

      <div class="footer__tradeview-markets">
        <b>Tradeview Markets</b> | Grand Cayman, KY1-1002, 4th Floor Harbour
        Place | 103 South Church St, PO Box 1105 Main Oﬃce: +1 345 945 6271
        Direct Phone: +1 345 946 4532 Website: www.tvmarkets.com
      </div>
    </section>
    <section>
      <div>
        <div>
          <p>
            Find daily trading insights and understand what is behind the latest
            waves in financial markets.
          </p>
          <img
            src="https://www.tvmarkets.com/_nuxt/img/surfs-up-gray.e67323f.svg"
            alt=""
          />
          <div class="separator"></div>
        </div>
        <div>
          <input type="text" />
          <AppMainButton text="Subscribe" type="filled" activeColor="#4B4D5C" />
        </div>
      </div>
      <div>
        <nav>
          <ul>
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
        <div>
          <nav>
            <h3>ACCOUNTS</h3>
            <ul>
              <li><a href="">Open account</a></li>
              <li><a href="">Individual</a></li>
              <li><a href="">Joint</a></li>
              <li><a href="">Corporate</a></li>
            </ul>
          </nav>
          <nav>
            <h3>ABOUT TRADEVIEW</h3>
            <ul>
              <li><a href="">Our Story</a></li>
              <li><a href="">Our Team</a></li>
              <li><a href="">Our Vision</a></li>
            </ul>
          </nav>
          <nav>
            <h3>COMPANY</h3>
            <ul>
              <li><a href="">Why Tradeview</a></li>
              <li><a href="">Sponsorships</a></li>
              <li><a href="">Press</a></li>
            </ul>
          </nav>
        </div>
        <div>
          <nav>
            <h3>SOFTWARE</h3>
            <ul>
              <li><a href="">MetaTrader 4</a></li>
              <li><a href="">MetaTrader 5</a></li>
              <li><a href="">cTrader</a></li>
              <li><a href="">cTrader Copy</a></li>
              <li><a href="">CurreneX</a></li>
            </ul>
          </nav>
          <nav>
            <h3>SUPPORT</h3>
            <ul>
              <li><a href=""> Forms and Documents </a></li>
              <li><a href="">FAQ</a></li>
            </ul>
          </nav>
        </div>
      </div>
    </section>
    <FooterLegalDeclarations />
  </footer>
</template>

<style scoped>
.footer {
  background-color: var(--dark-gray-bg);
}
</style>
