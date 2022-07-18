<template>
  <v-app-bar
    fixed
    color="white"
    outline
    class="header"
    elevate-on-scroll
    scroll-target="#scrolling-techniques-7"
  >
    <nuxt-link to="/">
      <v-img
        :src="require('~/assets/logo.png')"
        max-height="24"
        max-width="114"
      />
    </nuxt-link>

    <v-spacer></v-spacer>

    <v-list class="d-flex">
      <v-list-item v-for="item in items" :key="item.title" :to="item.to">
        <v-list-item-title class="text-center" v-text="item.title" />
      </v-list-item>
    </v-list>
  </v-app-bar>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          title: 'Home',
          to: '/',
        },
        {
          title: 'About Us',
          to: '/About',
        },
        {
          title: 'Services',
          to: '/Services',
        },
        {
          title: 'Contact Us',
          to: '/Contact',
        },
      ],
    }
  },
}
</script>

<style lang="scss">
.header {
  height: auto;
}

.v-application--wrap {
  height: auto !important;
  min-height: auto;
  flex: none;
  width: 100%;
}

.v-list {
  padding: 0;
}
</style>
