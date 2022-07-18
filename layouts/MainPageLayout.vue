<template>
  <v-app>
    <HeaderComp />
    <v-main id="scrolling-techniques-7">
      <Nuxt />
    </v-main>
    <Footer />
  </v-app>
</template>

<script>
import HeaderComp from '@/components/Header-comp'
import Footer from '@/components/Footer'
export default {
  name: 'MainPageLayout',
  component: { HeaderComp, Footer },
  data() {
    return {}
  },
}
</script>
<style>
@media (min-width: 1264px) {
  .lg-container {
    max-width: 1400px;
  }
}
</style>
