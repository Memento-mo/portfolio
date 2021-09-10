<template>
  <Section>
    <template v-slot:background>
      <div>experience</div>
    </template>

    <template v-slot:body>
      <p>
        опыт
      </p>
    </template>

    <div class="experience">
      <div>
        <!-- icon -->
      </div>
      <div class="experience__text">
        <div class="experience__text-title">
          ExactFarming - Frontend Developer (Сентябрь 2020 - По настоящее)
        </div>
        <div class="experience__text-description">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae explicabo, repudiandae nobis accusamus labore consequuntur sunt! Minima laboriosam ipsa labore! Quo, optio. Velit numquam eius aspernatur. Suscipit quisquam mollitia voluptates saepe aliquid ipsa. Saepe sunt veniam, commodi deleniti magni maxime eveniet deserunt assumenda, voluptatibus ratione fugiat. Eligendi facere ab sed.
        </div>
      </div>

      <div class="line" />

      <div class="experience__text">
        <div class="experience__text-title">
          AT Consulting - Intern JavaScript Developer (Декабрь 2018 - Февраль 2019)
        </div>
        <div class="experience__text-description">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae explicabo, repudiandae nobis accusamus labore consequuntur sunt! Minima laboriosam ipsa labore! Quo, optio. Velit numquam eius aspernatur. Suscipit quisquam mollitia voluptates saepe aliquid ipsa. Saepe sunt veniam, commodi deleniti magni maxime eveniet deserunt assumenda, voluptatibus ratione fugiat. Eligendi facere ab sed.
        </div>
      </div>
    </div>
  </Section>
</template>

<script lang="ts">
import { defineComponent } from '@vue/runtime-core'

import Section from '@/components/wrapper/Section.vue'


export default defineComponent({
  components: {
    Section
  }
})
</script>

<style lang="stylus" scoped>
.experience {
  margin-top 4rem
  &__text {

    &-title {
      font-weight 600
      font-size 2rem
    }  

    &-description {
      margin-top 1rem
      font-size 1.2rem
      opacity var(--opacity-text)
      line-height 2.2rem
    }
  }
}

</style>
