<template>
  <main>
    <section>
      <ExperienceBody />
    </section>
  </main>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

import ExperienceBody from '@/containers/Experience/ExperienceBody.vue'

export default defineComponent({
  components: {
    ExperienceBody
  }
})
</script>
