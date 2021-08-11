<template>
  <div class="cards">
    <div class="card">
      <Card title="spa app" message="Создание одностраничных и многофункциональных приложений">
        <template v-slot:icon>
          <Spa height="30" width="30"/>
        </template>
      </Card>
    </div>

    <div class="card">
      <Card title="wep app" message="Верстка лендингов и сайтов">
        <template v-slot:icon>
          <Spa height="30" width="30"/>
        </template>
      </Card>
    </div>

    <div class="card">
      <Card title="ui design" message="Разработка дизайна приложения">
        <template v-slot:icon>
          <Spa height="30" width="30"/>
        </template>
      </Card>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

import Card from '@/components/Card.vue'
import Spa from '@/icons/Spa.vue'

export default defineComponent({
  components: {
    Card,
    Spa
  }
})
</script>

<style lang="stylus" scoped>
  .cards {
    margin-top 10rem
    display flex
    justify-content center
    gap 30px
  }
</style>
