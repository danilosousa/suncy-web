<template>
  <div>
    <div class="wapp-bg">
      <Header />
      <v-container>
        <v-row justify="center" align="center">
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
        </v-row>
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
      height: 562px;
      width: 980px;
      display: block;
      position: absolute;
      top: 0;
      z-index: -1;

    }
  }
</style>
