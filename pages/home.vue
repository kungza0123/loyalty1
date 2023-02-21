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
      <v-container style="height: 1000px">
        <v-container fluid>
      <v-layout row wrap>
        <v-flex xs12 sm6 md4 lg3 v-for="item in newsItems" :key="item.id">
          <v-card>
            <v-img :src="item.image" aspect-ratio="1"></v-img>
            <v-card-title>{{ item.title }}</v-card-title>
            <v-card-text>{{ item.content }}</v-card-text>
            <v-card-actions>
              <v-btn text color="primary">Read more</v-btn>
            </v-card-actions>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
      </v-container>
    </v-sheet>
    
  </v-app>
</template>

  
  <script>
  export default {
    data() {
      return {
        newsItems: [
          {
            id: 1,
            title: 'Lorem ipsum dolor sit amet',
            content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. Praesent libero. Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at nibh elementum imperdiet. Duis sagittis ipsum. Praesent mauris. Fusce nec tellus sed augue semper porta. Mauris massa.',
            image: 'https://via.placeholder.com/400x400',
          },
          {
            id: 2,
            title: 'Pellentesque nec ipsum nec dolor',
            content: 'Pellentesque nec ipsum nec dolor dignissim convallis. Donec sit amet ligula enim. Duis vel nibh at velit scelerisque suscipit. Sed augue ipsum, egestas nec, vestibulum et, malesuada adipiscing, dui. In vel dui.',
            image: 'https://via.placeholder.com/400x400',
          },
          {
            id: 3,
            title: 'Vestibulum ante ipsum primis in faucibus orci',
            content: 'Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; In ac dui quis mi consectetuer lacinia. Nam pretium turpis et arcu. Duis arcu tortor, suscipit eget, imperdiet nec, imperdiet iaculis, ipsum.',
            image: 'https://via.placeholder.com/400x400',
          },
          {
            id: 4,
            title: 'Morbi in sem quis dui placerat ornare',
            content: 'Morbi in sem quis dui placerat ornare. Pellentesque odio nisi, euismod in, pharetra a, ultricies in, diam. Sed arcu. Cras consequat. Praesent dapibus, neque id cursus faucibus, tortor neque egestas augue, eu vulputate magna eros eu erat.',
            image: 'https://via.placeholder.com/400x400',
          }
        ]
      }
    }
  }
  </script>
  