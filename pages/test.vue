<template>
    <v-app id="inspire">
        <v-overlay :value="drawer" z-index="4">
    </v-overlay>
    <v-navigation-drawer v-model="drawer" app clipped hide-overlay :style="{ top: $vuetify.application.top + 'px', zIndex: 6 }">
      <v-list dense>
        <v-spacer></v-spacer>
        <v-list-item @click="d">
            News feed
        </v-list-item>
        <v-spacer></v-spacer>
        <v-list-item @click="f">
            Consign, Reward, Stars point
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
      <v-app-bar
        app
        color="#B22222"
        dark
        src="https://picsum.photos/1920/1080?random"
        fade-img-on-scroll
        shrink-on-scroll
      >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"> </v-app-bar-nav-icon>
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
      data() {
        return {
          drawer: false
        }
      },
    };
</script>

<style>
 main{
    background-color: #000000;
    /*background-image: url('./assets/banner.jpg'); */
 }
   
</style>

