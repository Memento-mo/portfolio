<template>
  <main>
    <section>
      <ServicesBody />
    </section>
    <section>
      <ServicesCards />
    </section>
  </main>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

import ServicesCards from '@/containers/Services/ServicesCards.vue'
import ServicesBody from '@/containers/Services/ServicesBody.vue'

export default defineComponent({
  components: {
    ServicesBody,
    ServicesCards
  }
})
</script>
