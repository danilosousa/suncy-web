<template>
  <v-app>
    <div class="wapp-bg">
      <Header />
      <v-container>
        <v-row>
          <v-col cols="5" sm="6" md="6">
            <div class="box">
              <div class="box__title">
                <!-- <h1>Sunsy</h1> -->
              </div>
              <div class="box__subtitle">
                <span><strong> A nova era dos eventos esportivos Organize divulgue,</strong>
                  gerencie sem complicação</span>
              </div>
              <div class="box__btns--actions">
                <CustomButton variant="secondary" btn-text="Registrar" />
                <CustomButton variant="transparent" btn-text="Compartilhar" />
              </div>
              <!-- <span class="box__description">
                April 24, 2022 Crown Hall, 05 Vineyard Drive, Ohio teste
              </span> -->
            </div>
          </v-col>
          <v-col cols="7" sm="6" md="6" class="box__video">
            <div class="box__video--wrapper" />
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
  </v-app>
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
      height: 710px;
      width: 1170px;
      display: block;
      position: absolute;
      top: 0;
      z-index: -1;
      background-size: 90%;
    }
    .box {
      height: 500px;
      display: flex;
      // align-items: center;
      justify-content: center;
      flex-direction: column;
      padding-left: 50px;
      &__subtitle{
        font-size: 25px;
        text-transform: uppercase;
        color: #fff;
      }
      &__btns--actions{
        margin: 25px 0;
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 65%;

      }

      &__video {
        display: flex;
        justify-content: flex-end;
        align-items: center;
        &--wrapper {
          background: #E6E6E6;
          width: 550px;
          height: 450px;
          border-radius: 30px;
        }
      }
    }
  }
</style>
