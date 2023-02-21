<template>
  <v-app id="inspire">
    <v-overlay :value="drawer" z-index="4">
    </v-overlay>
    <v-navigation-drawer v-model="drawer" app clipped hide-overlay
      :style="{ top: $vuetify.application.top + 'px', zIndex: 6 }">
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
    <v-app-bar app color="#B22222" dark src="https://picsum.photos/1920/1080?random" fade-img-on-scroll shrink-on-scroll>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"> </v-app-bar-nav-icon>
      <v-app-bar-title>Loyalty Program</v-app-bar-title>
      <v-spacer></v-spacer>
    </v-app-bar>
    <v-container>
      <v-row>
        <v-col>
          <div class="d-flex align-center">
            <v-avatar color="#000000" size="40">
              <v-icon dark>mdi-arrow-left-circle</v-icon>
            </v-avatar>
          </div>
        </v-col>
      </v-row>
      <v-row>
        <v-col></v-col>
        <v-col align="center" justify="space-around">
          <div v-resize-text id="star" class="font-weight-black">
            <h4>You have star: {{ counter }} Stars</h4>
          </div>
          <div v-resize-text>
            <h5>If you want to consign stars.</h5>
          </div>
        </v-col><v-col></v-col>
      </v-row>
      <v-row>
        <v-col></v-col>
        <v-col align="center" justify="space-around">
          <v-btn>
            send stars
          </v-btn>
        </v-col><v-col></v-col>
      </v-row>
      <v-row>
        <v-col >

        </v-col>
      </v-row>
      <v-row>
        <v-col align="center" justify="space-around">
          <div v-resize-text>
            <h5>Reward Exchange :</h5>
          </div>
        </v-col><v-col></v-col>
      </v-row>

    </v-container>
    <v-sheet>
      <v-container>
        <v-row>

            <v-col cols="12" md="6" lg="4">
                <v-hover v-slot:default="{ hover }" open-delay="50" close-delay="50">
                  <div>
                    <v-card flat :color="hover ? 'white' : 'transparent'" :elevation="hover ? 12 : 0" hover to="/history">
                      <v-img
                        src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRa4xkBzGDQyj4D0ymgAdBqe9cFsbFYorqfSg&usqp=CAU"
                        :aspect-ratio="16 / 9" gradient="to top, rgba(25,32,72,.4), rgba(25,32,72,.0)" height="200px"
                        class="elevation-2" style="border-radius: 16px">
                        <!-- <v-card-text>
                          <v-btn color="accent">Sold out</v-btn>
                        </v-card-text> -->
                      </v-img>

                      <v-card-text>
                        <div class="text-h5 font-weight-bold primary--text">
                          Train Tracks
                        </div>

                        <div class="text-body-1 py-4">Description
                          'Nature with Train Tracks'

                          </div>
                        <div class="d-flex align-center">
                          <v-avatar color="accent" size="36">
                            <v-icon dark>mdi-star</v-icon>
                          </v-avatar>

                          <div class="pl-2">12.00</div>
                        </div>
                      </v-card-text>
                    </v-card>
                  </div>
                </v-hover>
              </v-col>

              <v-col cols="12" md="6" lg="4">
                <v-hover v-slot:default="{ hover }" open-delay="50" close-delay="50">
                  <div>
                    <v-card flat :color="hover ? 'white' : 'transparent'" :elevation="hover ? 12 : 0" hover to="/history">
                      <v-img
                        src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR1MY-Jyz53_qGn1eC-2FMx85R5F61Dm_TBZw&usqp=CAU"
                        :aspect-ratio="16 / 9" gradient="to top, rgba(25,32,72,.4), rgba(25,32,72,.0)" height="200px"
                        class="elevation-2" style="border-radius: 16px">
                        <!-- <v-card-text>
                          <v-btn color="accent">Sold out</v-btn>
                        </v-card-text> -->
                      </v-img>

                      <v-card-text>
                        <div class="text-h5 font-weight-bold primary--text">
                          Leaf
                        </div>

                        <div class="text-body-1 py-4">Description
                          'Drop of wateron leaf'

                          </div>
                        <div class="d-flex align-center">
                          <v-avatar color="accent" size="36">
                            <v-icon dark>mdi-star</v-icon>
                          </v-avatar>

                          <div class="pl-2">24.12</div>
                        </div>
                      </v-card-text>
                    </v-card>
                  </div>
                </v-hover>
              </v-col>

              <v-col cols="12" md="6" lg="4">
                <v-hover v-slot:default="{ hover }" open-delay="50" close-delay="50">
                  <div>
                    <v-card flat :color="hover ? 'white' : 'transparent'" :elevation="hover ? 12 : 0" hover to="/history">
                      <v-img
                        src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSfvhC52821-wSuPOn7jA2pZXSzzY15HnSPiA&usqp=CAU"
                        :aspect-ratio="16 / 9" gradient="to top, rgba(25,32,72,.4), rgba(25,32,72,.0)" height="200px"
                        class="elevation-2" style="border-radius: 16px">
                        <!-- <v-card-text>
                          <v-btn color="accent">Sold out</v-btn>
                        </v-card-text> -->
                      </v-img>

                      <v-card-text>
                        <div class="text-h5 font-weight-bold primary--text">
                          Lake
                        </div>

                        <div class="text-body-1 py-4">Description
                          'Mountain of the lake'

                          </div>
                        <div class="d-flex align-center">
                          <v-avatar color="accent" size="36">
                            <v-icon dark>mdi-star</v-icon>
                          </v-avatar>

                          <div class="pl-2">48.24</div>
                        </div>
                      </v-card-text>
                    </v-card>
                  </div>
                </v-hover>
              </v-col>

        </v-row>
      </v-container>
    </v-sheet>
  </v-app>
</template>

<script>
import ResizeText from 'vue-resize-text'
export default {
  directives: {
    ResizeText
  },
  data() {
    return {
      drawer: false,
      counter: 0.00
    }
  },
};
</script>

<style>
main {
  background-image: url('../img/back.png');
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
}</style>