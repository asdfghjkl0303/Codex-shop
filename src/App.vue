<script setup>
import SiteHeader from './components/SiteHeader.vue'
import SeasonalMenu from './components/SeasonalMenu.vue'
</script>

<template>
  <SiteHeader />

  <main>
    <section class="hero" aria-labelledby="hero-title">
      <div class="hero-photo" role="img" aria-label="温暖灯光下摆放着当季中式佳肴的餐桌"></div>
      <div class="hero-shade"></div>
      <div class="hero-content">
        <p class="eyebrow light"><span></span> SEASONAL CUISINE · HANGZHOU</p>
        <h1 id="hero-title">一席之间，<br /><em>见山见味。</em></h1>
        <p class="hero-desc">循着四时风物，把山野的鲜、灶火的暖，<br class="desktop-break" />做成一桌值得慢慢吃的家常菜。</p>
        <div class="hero-actions"><a class="button button-light" href="#menu">看看当季菜单 <span>↓</span></a><a class="text-link light-link" href="#story">认识见山 <span>↗</span></a></div>
      </div>
      <div class="hero-caption"><span>01 — 04</span><span>当季 · 初秋丰味</span></div>
      <div class="hero-vertical">GOOD FOOD, GOOD SEASONS</div>
    </section>

    <section class="intro section-pad" id="story">
      <div class="intro-mark" aria-hidden="true">山<br />野<br /><i>之<br />间</i></div>
      <div class="intro-copy">
        <p class="eyebrow"><span></span> A TABLE WITH THE SEASONS</p>
        <h2>好好吃饭，<br />也好好感受<span>四季。</span></h2>
        <p class="body-copy">见山相信，味道自有来处。清晨采来的时蔬、溪涧长大的鲜鱼，还有一口慢慢熬开的老汤——我们把对土地的珍惜，做进每天的菜单里。</p>
        <a class="text-link" href="#space">关于见山小馆 <span>↗</span></a>
      </div>
      <div class="intro-photo-wrap"><img src="https://images.unsplash.com/photo-1547592180-85f173990554?auto=format&fit=crop&w=1000&q=85" alt="新鲜蔬菜和香料铺满木桌" loading="lazy" /><span class="photo-note">从田间，到餐桌<br /><small>FROM FARM TO TABLE</small></span></div>
    </section>

    <SeasonalMenu />

    <section class="quote-band" id="space"><div class="quote-image"></div><div class="quote-content"><span class="quote-mark">“</span><p>山不在远，<br />好味就在<span>眼前。</span></p><small>让每一次相聚，都有好好吃饭的理由。</small><a class="text-link light-link" href="#visit">来见山坐坐 <span>↗</span></a></div><span class="quote-side">GATHER · EAT · STAY A WHILE</span></section>

    <section class="visit-section section-pad" id="visit">
      <div class="visit-title"><p class="eyebrow"><span></span> COME FIND US</p><h2>留一张桌，<br />等你来<span>见山。</span></h2><p>一餐一饭，一期一会。<br />想来的时候，记得提前留个位子。</p><a class="button button-dark" href="tel:057186680218">电话预订 <span>↗</span></a></div>
      <div class="visit-details"><div class="detail-block"><span class="detail-label">找到我们</span><p>杭州市 · 西湖区<br />青芝坞 28 号 · 见山小馆</p><a class="text-link" href="https://maps.google.com/?q=Hangzhou+Qingzhiwu" target="_blank" rel="noreferrer">查看地图 <span>↗</span></a></div><div class="detail-block"><span class="detail-label">营业时间</span><p>午市 11:00 — 14:00<br />晚市 17:00 — 21:30</p><span class="detail-muted">每周一休息 · 节假日照常营业</span></div><div class="detail-block"><span class="detail-label">电话预约</span><p class="phone-number">0571 — 8668 0218</p><span class="detail-muted">也欢迎直接到店，碰个好时候。</span></div></div>
    </section>
  </main>
  <footer class="site-footer"><a class="brand footer-brand" href="#top"><span class="brand-seal">見</span><span class="brand-copy"><strong>见山小馆</strong><small>JIÀN SHĀN · SEASONAL KITCHEN</small></span></a><span>好好吃饭，四季见山。</span><span>© 2025 见山小馆</span></footer>
</template>
