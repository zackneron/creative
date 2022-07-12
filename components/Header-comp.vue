<template>
  <v-app-bar color="white">
    <nuxt-link to="/">
      <v-img
        :src="require('~/assets/logo.png')"
        max-height="24"
        max-width="114"
      />
    </nuxt-link>

    <v-spacer></v-spacer>

    <v-list class="d-none d-sm-flex">
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
          title: 'Whats New',
          to: '/whats-new',
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

<style></style>
