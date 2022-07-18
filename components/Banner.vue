<template>
  <div class="hero">
    <v-container class="lg-container">
      <v-row justify="center" align="center">
        <v-col cols="12">
          <div class="hero__content text-center">
            <h1 class="hero__title white--text mb-8 text-h3">{{ title }}</h1>
            <h2 class="text-h5 white--text font-weight-light">
              {{ description }}
            </h2>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: 'Hero',
  props: {
    title: {
      type: String,
      required: true,
    },
    description: {
      type: String,
      required: true,
    },
  },
}
</script>

<style lang="scss">
.hero {
  background: #26b186;
  padding: 100px 50px 50px;
  &__content {
    margin: auto;
  }
  &__title {
    text-shadow: 2px 2px rgba(0, 0, 0, 0.6);
  }
}
</style>
