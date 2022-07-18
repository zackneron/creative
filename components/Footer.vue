<template>
  <v-footer class="footer">
    <v-container fluid>
      <v-row justify="center" align="center">
        <v-col cols="12">
          <div class="text-center">
            <span class="caption">Copyright &copy; 2022 Katshi Way Design</span>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-footer>
</template>
<script>
export default {
  name: 'Footer',
  data() {
    return {}
  },
}
</script>

<style lang="scss">
.theme--light.v-footer {
  background-color: #737373;
  color: #fff;
}
</style>
