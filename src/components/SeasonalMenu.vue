<script setup>
const dishes = [
  { name: '桂花糖藕', description: '金秋桂香 · 手作糯米藕', price: '38', image: 'dish-one' },
  { name: '笋干老鸭煲', description: '慢火炖煮 · 暖胃好时节', price: '128', image: 'dish-two', featured: true },
  { name: '青梅小排', description: '酸甜梅香 · 鲜嫩入味', price: '68', image: 'dish-three' },
]
</script>

<template>
  <section class="menu-section section-pad" id="menu">
    <div class="section-heading"><div><p class="eyebrow"><span></span> WHAT'S IN SEASON</p><h2>此时此味<span>，正当时。</span></h2></div><p>时令不等人，好味道也是。<br />这些是我们最近最喜欢的几道。</p></div>
    <div class="menu-grid">
      <article v-for="(dish, index) in dishes" :key="dish.name" class="dish-card" :class="{ 'featured-dish': dish.featured }">
        <div class="dish-image" :class="dish.image"><span class="dish-index">{{ String(index + 1).padStart(2, '0') }}</span><span v-if="dish.featured" class="dish-tag">主厨推荐</span></div>
        <div class="dish-meta"><div><h3>{{ dish.name }}</h3><p>{{ dish.description }}</p></div><span class="dish-price">¥ {{ dish.price }}</span></div>
      </article>
    </div>
    <div class="menu-foot"><span>菜单随季节更替 · 每日鲜选</span><a class="text-link" href="#visit">探索完整菜单 <span>↗</span></a></div>
  </section>
</template>
