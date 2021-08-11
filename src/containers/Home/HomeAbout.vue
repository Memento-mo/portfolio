<template>
  <div class="about row justify-content-center flex-direction-column align-items-center">
    <div class="backtext backtext-addition">
      <div>I'm</div>
    </div>

    <div class="about-title">
      Frontend developer
    </div>

    <div class="about-photo">
      <img src="../../img/AirBrush_20210808212213.jpg" />
    </div>
  </div>
</template>

<style lang="stylus" scoped>
.about {
  margin-top 10rem
  text-align center
  position relative

  &-text {
    margin-right 5rem
  }

  &-message {
    font-size 5rem
    font-weight 300

    span {
      font-weight 600
    }
  }

  &-title {
    font-size 4rem
    font-weight 300
    text-transform uppercase
    letter-spacing 2px
    margin-bottom 2rem
  }

  &-photo {
    display flex
    justify-content center
    align-items center

    img {
      height 60rem
      border-radius 1rem
      box-shadow var(--shadow)
      cursor pointer
      backface-visibility hidden

      transition 0.3s ease

      &:hover {
        transform translateY(-1rem)
        box-shadow var(--hover-shadow)
      }
    }
    

    span {
      color grey
      text-transform uppercase
      font-size 4rem
    }
  }
}

.backtext-addition {
  left 25%
  top -12%
}
</style>