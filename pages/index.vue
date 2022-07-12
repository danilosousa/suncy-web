<template>
  <div>
    <div class="wapp-bg">
      <Header />
      <v-container>
        <v-row>
          <v-col cols="5" sm="6" md="6">
            <div class="box">
              <div class="box__title">
                Suncy
              </div>
              <div class="box__subtitle">
                The Biggest STRATEGY IN 2020
              </div>
              <div class="box__description" />
            </div>
          </v-col>
          <v-col cols="7" sm="6" md="6">
            picture here
          </v-col>
        </v-row>

        <!-- <v-row justify="center" align="center">
          <v-col cols="12" sm="8" md="6">
            <v-card>
              <v-card-title class="headline">
                fsfd Welcome to the Vuetify + Nuxt.js template
              </v-card-title>
              <v-card-text>
                <p>
                  Vuetify is a progressive Material Design component framework for
                  Vue.js. It was designed to empower developers to create amazing
                  applications.
                </p>
              </v-card-text>
              <v-card-actions>
                <v-spacer />
                <v-btn color="dark" nuxt to="/inspire">
                  Continue
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row> -->
      </v-container>
    </div>
    <Footer />
  </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>
<style lang="scss">
  .wapp-bg{
    position: relative;
    &:after {
      content: '';
      background: url('../assets/images/bg.svg') no-repeat;
      height: 690px;
      width: 1170px;
      display: block;
      position: absolute;
      top: 0;
      z-index: -1;
      background-size: 88%;

    }
  }
</style>
