<template>
  <div>
    <header class="header">
      <v-container>
        <v-row>
          <v-col md="3">
            <div class="logo">
              <Logo />
              <span class="logo-text">SUNSY</span>
            </div>
          </v-col>
          <v-col md="5">
            <nav class="header-nav">
              <ul>
                <li>
                  <a href="#">Home</a>
                  <a href="#">Quem somos</a>
                  <a href="#">Eventos</a>
                  <a href="#">Noticias</a>
                  <a href="#">Contato</a>
                </li>
              </ul>
            </nav>
          </v-col>
          <v-col md="4" class="d-flex align-center justify-end">
            <span class="header__icon-search">

              <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 15 15" width="15px" height="15px">
                <g id="surface70599895">
                  <path style=" stroke:none;fill-rule:nonzero;fill:rgb(90.588236%,29.803923%,23.529412%);fill-opacity:1;" d="M 6.300781 0.898438 C 3.484375 0.898438 1.199219 3.1875 1.199219 6 C 1.199219 8.8125 3.484375 11.101562 6.300781 11.101562 C 7.414062 11.101562 8.441406 10.742188 9.28125 10.132812 L 13.226562 14.070312 L 14.070312 13.226562 L 10.171875 9.320312 C 10.9375 8.425781 11.398438 7.265625 11.398438 6 C 11.398438 3.1875 9.113281 0.898438 6.300781 0.898438 Z M 6.300781 1.5 C 8.789062 1.5 10.800781 3.511719 10.800781 6 C 10.800781 8.488281 8.789062 10.5 6.300781 10.5 C 3.8125 10.5 1.800781 8.488281 1.800781 6 C 1.800781 3.511719 3.8125 1.5 6.300781 1.5 Z M 6.300781 1.5 " />
                </g>
              </svg>

            </span>
            <span>
              <!-- <button class="button button-main shadow">
                Publique
              </button> -->
              <CustomButton btn-text="Publique" />
            </span>
          </v-col>
        </v-row>
      </v-container>
    </header>
  </div>
</template>

<script>
// import { Client, Account } from 'appwrite'

export default {
  name: 'HeaderLayout',

  data () {
    return {
      // testex: ''
    }
  },
  methods: {
    // async teste () {
    //   const client = new Client()

    //   const account = new Account(client)

    //   client
    //     .setEndpoint('https://api.sunsy.io/v1') // Your API Endpoint
    //     .setProject('62c23e8c21a24f5b5a1a') // Your project ID

    //   const response = await account.createEmailSession(
    //     'email@example.com',
    //     'password'
    //   )
    //   console.log('response', response)
    // }
  }
}
</script>
<style lang="scss">
  button {
    &.button {
      background-color: #4CAF50; /* Green */
      border: none;
      color: #fff;
      font-weight: bold;
      padding: 10px 50px;
      text-align: center;
      text-decoration: none;
      display: inline-block;
      font-size: 14px;
      border-radius: 16px;
      transition-duration: 0.4s;
      cursor: pointer;
      &-main {
        background: transparent -webkit-linear-gradient(45deg, #ff0f7b, #f89c2a) repeat scroll 0 0;
      }
    }
  }

.header {
  // background: transparent -webkit-linear-gradient(45deg, #ff0f7b, #f89c2a) repeat
  //   scroll 0 0;

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

  &__icon-search{
    padding: 0 25px;
  }

  &-nav {
    display: flex;
    align-items: center;
    height: 70px;

    ul {
      width: 100%;
      li {
        display: flex;
        justify-content: space-evenly;
        font-size: 16px;
        a{
          color: #fff;
          text-decoration: none;
          font-weight: bold;
          font-weight: 400;
          font-size: 14px;
          &:hover {
            text-decoration: underline;
          }
        }
      }
    }
  }
}
</style>
