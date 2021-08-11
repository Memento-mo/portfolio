<template>
  <section class="header row">
    <div class="backtext backtext-addition">
      modern
    </div>
    <div class="preview">
      <span class="preview__subtitle">творю с любовью</span>
      <h1 class="preview__title">Кодинг & Разработка</h1>
      <p class="preview__message">Создание красивых, адаптивных и высокоотзывчивых SPA/WEB приложений</p>

      <div class="preview__icons">
        <div class="preview__icons-icon">
          <a href="https://vk.com/glebkkaa" target="_blank">
            <Vk height="24" width="24" />
          </a>
        </div>
        <div class="preview__icons-icon">
          <a href="https://t.me/gpolog" target="_blank">
            <Telegram height="18" width="18" />
          </a>
        </div>

        <div class="preview__icons-icon">
          <a href="https://github.com/Memento-mo" target="_blank">
            <Github height="18" width="18" />
          </a>
        </div>
      </div>
    </div>

    <div>
      <!-- logo -->
    </div>
  </section>
</template>

<script lang="ts">
import { defineComponent } from '@vue/runtime-core'

import Vk from '@/icons/Vk.vue'
import Telegram from '@/icons/Telegram.vue'
import Github from '@/icons/Github.vue'

export default defineComponent({
  components: {
    Vk,
    Telegram,
    Github
  }
})
</script>

<style lang="stylus" scoped>
.header {
  position relative
  margin-top 5rem

  .preview {
    flex-basis 60%

    &__title {
      font-size 6rem
      font-weight 600
      line-height 7rem
    }

    &__subtitle {
      color var(--hover-text)
      font-size 1.4rem
    }

    &__message {
      margin-top 2rem
      color var(--grey-1)
      font-size 1.4rem 
    }

    &__icons {
      display flex
      align-items center
      margin-top 2.5rem

      &-icon {
        margin-right 2rem
      }
    }
  }
}

.backtext-addition {
  top -20%
  left 1%
}
</style>
