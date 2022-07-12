<template>
  <div>
    <button class="button button-main shadow">
      <slot> {{ btnText }}</slot>
    </button>
  </div>
</template>

<script>
export default {
  props: {
    btnText: {
      type: String,
      default () {
        return ''
      }
    }
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
</style>
