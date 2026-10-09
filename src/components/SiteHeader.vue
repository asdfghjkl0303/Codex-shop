<script setup>
import { ref } from 'vue'

const menuOpen = ref(false)
const navigation = [
  { label: '关于见山', href: '#story' },
  { label: '当季菜单', href: '#menu' },
  { label: '餐厅空间', href: '#space' },
  { label: '联系我们', href: '#visit' },
]

function closeMenu() {
  menuOpen.value = false
}
</script>

<template>
  <header class="site-header" id="top">
    <a class="brand" href="#top" aria-label="见山小馆首页" @click="closeMenu">
      <span class="brand-seal">見</span>
      <span class="brand-copy"><strong>见山小馆</strong><small>JIÀN SHĀN · SEASONAL KITCHEN</small></span>
    </a>
    <button
      class="menu-toggle"
      type="button"
      :aria-label="menuOpen ? '关闭导航' : '打开导航'"
      :aria-expanded="menuOpen"
      aria-controls="main-navigation"
      @click="menuOpen = !menuOpen"
    ><span></span><span></span></button>
    <nav id="main-navigation" class="main-nav" :class="{ open: menuOpen }" aria-label="主导航">
      <a v-for="item in navigation" :key="item.href" :href="item.href" @click="closeMenu">{{ item.label }}</a>
      <a class="nav-booking" href="#visit" @click="closeMenu">预订座位 <span>↗</span></a>
    </nav>
  </header>
</template>
