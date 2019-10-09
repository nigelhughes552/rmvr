<template>
  <v-app>
    <v-app-bar :clipped-left="clipped" fixed app color="blue-grey lighten-4">
      <v-toolbar-title v-text="title" />
    </v-app-bar>
    <v-content>
      <v-container fluid>
        <nuxt />
      </v-container>
    </v-content>

    <v-footer :fixed="fixed" app>
      <span>&copy; RMVR 2019</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      fixed: false,
      clipped: false,
      title: 'RMVR'
    }
  }
}
</script>
