<template>
  <button
    class="button shadow"
    :class="btnStyle"
  >
    <slot> {{ btnText }}</slot>
  </button>
</template>

<script>
export default {
  props: {
    variant: {
      type: String,
      default: ''
    },
    btnText: {
      type: String,
      default () {
        return ''
      }
    }
  },
  data () {
    return {

    }
  },
  computed: {
    btnStyle () {
      switch (this.variant) {
        case 'main':
          return 'button-main'
        case 'secondary':
          return 'button-secondary'
        case 'transparent':
          return 'button-transparent'
        default:
          return ''
      }
    }
  }
}
</script>

<style lang="scss">
  button {
    &.button {
      min-width: 150px;
      width: 150px;
      border: none;
      color: #fff;
      font-weight: bold;
      padding: 10px 0;
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
      &-secondary{
        background: #fff;
        color: #000;
      }
      &-transparent {
        background: transparent;
        color: #fff;
        border: 1px solid #fff;
      }
    }
  }
</style>
