<template>
  <v-app>
    <HeaderComp />
    <v-main>
      <Nuxt />
    </v-main>
    <Footer />
  </v-app>
</template>

<script>
import HeaderComp from '@/components/Header-comp'
import Footer from '@/components/FooterCom'
export default {
  name: 'MainPageLayout',
  component: { HeaderComp, Footer },
  data() {
    return {}
  },
}
</script>
<style scoped></style>
