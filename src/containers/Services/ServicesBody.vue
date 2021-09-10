<template>
  <Section>
    <template v-slot:background>
      <div>my</div>
      <div>services</div>
    </template>

    <template v-slot:body>
      <div class="row align-items-center">
        <div class="services-body__title">
          <p>сервисы</p>
        </div>
        <div class="services-body__text">
          <p>Только современная разработка</p>
        </div>
      </div>
    </template>
  </Section>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

import Section from '@/components/wrapper/Section.vue'

export default defineComponent({
  components: {
    Section
  }
})
</script>

<style lang="stylus" scoped>
.services-body {
  position relative
  max-width 70%
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
  top -150%
  left 2%
}
</style>
