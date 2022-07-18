<template>
  <v-app>
    <HeaderComp />
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <FooterComp />
  </v-app>
</template>

<script>
import HeaderComp from '@/components/Header-comp'
import FooterComp from '@/components/Footer'
export default {
  name: 'DefaultLayout',
  component: { HeaderComp, FooterComp },
  data() {
    return {}
  },
}
</script>
