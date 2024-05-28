<template>
  <div class="home-container">
    <app-navbar4></app-navbar4>
    <app-hero9></app-hero9>
    <app-features1></app-features1>
    <app-contact3></app-contact3>
    <app-footer1></app-footer1>
  </div>
</template>

<script>
import AppNavbar4 from '../components/navbar4'
import AppHero9 from '../components/hero9'
import AppFeatures1 from '../components/features1'
import AppContact3 from '../components/contact3'
import AppFooter1 from '../components/footer1'

export default {
  name: 'Home',
  props: {},
  components: {
    AppNavbar4,
    AppHero9,
    AppFeatures1,
    AppContact3,
    AppFooter1,
  },
  head: {
    title: 'Flowery Slow Pigeonpppp',
    meta: [
      {
        property: 'og:title',
        content: 'Flowery Slow Pigeonpppp',
      },
    ],
  },
}
</script>

<style scoped>
.home-container {
  width: 100%;
  display: flex;
  min-height: 100vh;
  align-items: center;
  flex-direction: column;
}
</style>
