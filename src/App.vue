<script setup lang="ts">
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
</script>

<template>
  <div class="main-home-view">
    <Header />
    <RouterView />
    <Footer />
  </div>
</template>

<style lang="scss">
.main-home-view {
  display: flex;
  flex-direction: column;
  padding: 0 10vw;
}
</style>
