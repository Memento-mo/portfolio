<template>
  <div class="card">
    <div class="card-header">
      <div class="card-header__icon">
        <slot name="icon" />
      </div>
      <div class="card-header__title">
        <slot name="title" />
        {{ title }}
      </div>
    </div>
    <div class="card-header__message">
      {{ message }}
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from '@vue/runtime-core'
export default defineComponent({
  props: {
    title: String,
    message: String
  }
})
</script>

<style lang="stylus" scoped>
.card {
  max-width 200px
  width 100
  background var(--secondary)
  box-shadow var(--shadow)

  padding 2rem
  border-radius 15px

  &-header {
    display flex
    align-items center

    &__title {
      margin-left 15px
      font-size 2rem
      font-weight 600  
    }

    &__message {
      margin-top 8px
      line-height 17px
      opacity 0.6
    }
  }

  transition 0.3s ease
  backface-visibility hidden
  cursor pointer

  &:hover {
    box-shadow var(--hover-shadow)
    transform translateY(-10px)
  }
}
</style>
