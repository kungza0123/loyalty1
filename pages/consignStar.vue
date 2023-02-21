<template>
  <v-app>
    <v-app-bar
      app
      color="#B22222"
      dark
      icon="menu"
      on-click="openDrawer"
      src="https://picsum.photos/1920/1080?random"
      fade-img-on-scroll
      shrink-on-scroll
    >
      <v-app-bar-nav-icon> </v-app-bar-nav-icon>
      <v-app-bar-title>Title</v-app-bar-title>
      <v-spacer></v-spacer>
    </v-app-bar>
    <v-sheet>
      <v-container style="height: 1000px"> </v-container>
    </v-sheet>
  </v-app>
</template>

<script>
export default {

}
</script>

<style>

</style>