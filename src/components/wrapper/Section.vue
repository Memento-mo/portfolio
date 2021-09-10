<template>
  <div class="body">
    <div class="row align-items-center">
      <div class="backtext backtext-addition">
          <slot name="background" />
      </div>
      <div class="body__title">
        <slot name="body" />
      </div>
    </div>

    <slot />
  </div>
</template>

<style lang="stylus" scoped>
.body {
  position relative
  max-width 90%
  margin 7rem auto 3rem auto

  &__title {
    font-size 4rem
    font-weight 300
    margin-right 3rem
  }

  &__text {
    font-size 1.2rem
    opacity var(--opacity-text)
    line-height 2.5rem
    margin-top 1rem
  }
}

.backtext-addition {
  font-size 14rem
  line-height 12rem
  
  left 2%
}
</style>
