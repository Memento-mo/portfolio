<template>
  <main class="container">
    <header>
      <Header />
    </header>

    <!-- <router-view v-slot="{ Component }">
      <transition name="scale" mode="out-in">
        <component :is="Component" />
      </transition>
    </router-view> -->
    <section>
      <Home />
    </section>
    
    <section class="padding">
      <Services />
    </section>

    <section class="padding">
      <Experience />
    </section>
  </main>
</template>

<script lang="ts">
import { defineComponent } from '@vue/runtime-core'

import Header from '@/components/Header.vue'

import Home from '@/views/Home.vue'
import Services from '@/views/Services.vue'
import Experience from '@/views/Experience.vue'

export default defineComponent({
  components: {
    Header,
    Home,
    Services,
    Experience
  }
})
</script>


<style lang="stylus" scoped>
.padding {
  padding-top 10rem
}
</style>
