<template>
  <div>
    <div class="hero">
      <v-container class="lg-container">
        <v-row justify="center" align="center">
          <v-col cols="12" sm="6" md="5">
            <h1>Your Trusted Strategy and Technology Partner</h1>
            <p>
              Empowering industry leaders through innovative business solutions
            </p>
          </v-col>
          <v-col cols="12" sm="6" md="7"></v-col>
        </v-row>
      </v-container>
    </div>
    <div class="service">
      <v-container class="lg-container">
        <v-row justify="center" align="center">
          <v-col cols="12" sm="6" md="3">Text 1</v-col>
          <v-col cols="12" sm="6" md="3">Text 2</v-col>
          <v-col cols="12" sm="6" md="3">Text 3</v-col>
          <v-col cols="12" sm="6" md="3">Text 4</v-col>
        </v-row>
      </v-container>
    </div>
    <div class="service">
      <v-container class="lg-container">
        <v-row justify="center" align="center">
          <v-col cols="12" sm="6" md="3">Text 1</v-col>
          <v-col cols="12" sm="6" md="3">Text 2</v-col>
          <v-col cols="12" sm="6" md="3">Text 3</v-col>
          <v-col cols="12" sm="6" md="3">Text 4</v-col>
        </v-row>
      </v-container>
    </div>
    <div class="service">
      <v-container class="lg-container">
        <v-row justify="center" align="center">
          <v-col cols="12" sm="6" md="3">Text 11</v-col>
          <v-col cols="12" sm="6" md="3">Text 2</v-col>
          <v-col cols="12" sm="6" md="3">Text 3</v-col>
          <v-col cols="12" sm="6" md="3">Text 4</v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  layout: 'MainPageLayout',
}
</script>
<style scoped>
.lg-container {
  padding: 0;
}
@media (min-width: 1264px) {
  .container {
    max-width: 1400px;
  }
}
.hero {
  background: lightblue;
  padding: 100px 50px;
}
.service {
  background: rgb(102, 157, 129);
  padding: 100px 50px;
}
</style>
