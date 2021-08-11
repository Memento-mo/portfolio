<template>
  <main>
    <section>
      <HomeHeader />
    </section>
    <section>
      <HomeAbout />
    </section>
  </main>
</template>

<script lang="ts">
import { defineComponent } from '@vue/runtime-core'

import HomeHeader from '@/containers/Home/HomeHeader.vue'
import HomeAbout from '@/containers/Home/HomeAbout.vue'

export default defineComponent({
  components: {
    HomeHeader,
    HomeAbout
  }
})
</script>
