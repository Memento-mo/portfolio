<template>
  <div class="header">
    <div class="row justify-content-between align-items-center">
      <div class="logo">
          Gleb Pologov
      </div>
      <nav class="navigation">
        <ul class="row">
          <li>
            <router-link to="/">Обо мне</router-link>
          </li>
          <li>
            <router-link to="/services">
              Сервисы
            </router-link>
          </li>
          <li>Опыт</li>
          <li>Инструменты</li>
          <li>Контакты</li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<style lang="stylus" scoped>
.logo {
  text-transform uppercase
  letter-spacing 5px
  font-size 1.4rem
  cursor pointer
}
.header {
  padding-top 8rem
  padding-bottom 6rem
}
.navigation {
  li {
    list-style-type none
    font-family Montserrat, sans-serif
    text-transform uppercase
    font-weight 300

    margin-right 1rem
    font-size 1rem
    letter-spacing 1px
    cursor pointer
    position relative
    transition 0.3s ease

    &:hover {
      color var(--hover-text)
    }
  }
}

.router-link-exact-active {
  color var(--hover-text)
}
</style>