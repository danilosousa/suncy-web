<template>
  <header class="header">
    <v-container>
      <v-row>
        <v-col md="2">
          <div class="logo">
            <Logo />
            <span class="logo-text">SUNSY</span>
          </div>
        </v-col>
        <v-col md="8">
          <nav class="header-nav">
            <ul>
              <li>
                <a href="#">Home</a>
                <a href="#">Sobre a SUNSY</a>
                <a href="#">Contato</a>
                <a href="#">Publique</a>
              </li>
            </ul>
          </nav>
        </v-col>
        <v-col md="2">
          <span>Lupa</span>
          <span>Publique</span>
        </v-col>
      </v-row>
    </v-container>
  </header>
</template>
<script>
// import Logo from '@src/assets/iamges/logo.svg'

export default {
  name: 'HeaderLayout'
  // components: Logo
}
</script>
<style lang="scss">
.header {
  background: transparent -webkit-linear-gradient(45deg, #ff0f7b, #f89c2a) repeat
    scroll 0 0;
  .logo {
    align-items: center;
    justify-content: flex-start;
    display: flex;
    svg {
      width: 60px;
      height: 60px;
    }
    &-text {
      font-size: 18px;
      padding-left: 10px;
      color: #fff;
      font-weight: bold;
    }
  }
  &-nav {
    display: flex;
    align-items: center;
    height: 80px;

    ul {
      width: 100%;
      li {
        display: flex;
        justify-content: space-evenly;
      }
    }
  }
}
</style>
