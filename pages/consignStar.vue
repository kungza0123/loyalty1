<template>
  <v-app>
    <v-app-bar
      app
      color="grey"
      dark
      prominent
      src="https://picsum.photos/1920/1080?random"
      fade-img-on-scroll
      shrink-on-scroll
    >
      <v-app-bar-nav-icon> </v-app-bar-nav-icon>
      <v-app-bar-title>Title</v-app-bar-title>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
      <v-menu left bottom>
        <template v-slot:activator="{ on, attrs }">
          <v-btn icon v-bind="attrs" v-on="on">
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </template>
      </v-menu>
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