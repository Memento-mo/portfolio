<template>
  <div
    class="logo"
    :style="{ height: height + 'rem', width: width + 'rem' }"
  >
    <div :style="{ height: height - 1 + 'rem', width: width - 1 + 'rem' }" class="logo-inside" />
  </div>
</template>

<script>
export default {
  props: {
    height: {
      required: true,
      type: Number,
      default: 3
    },
    width: {
      required: true,
      type: Number,
      default: 3
    }
  }
}
</script>

<style lang="stylus" scoped>
.logo {
  background-color transparent
  border-radius 50%
  border .6rem solid #fff
  border-bottom-color transparent

  .logo-inside {
    border-radius 50%
    border .6rem solid #fff
    border-top-color transparent
    border-left-color transparent
    border-right-color transparent
    position relative
    top 5px
    left -1.5px
  }
}
</style>