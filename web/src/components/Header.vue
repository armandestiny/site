<template>
  <div class="wrapper">
    <nav>
      <router-link to="/">Главная</router-link>
      <router-link to="/about">О нас</router-link>
      <router-link to="/OurProduct">Наш продукт</router-link>
      <router-link to="/News">Ассортимент</router-link>
      <router-link to="/News">Новости/Акции</router-link>
      <router-link to="/QA">Вопросы/Ответы</router-link>
      <router-link to="/News">Доставка и оплата</router-link>
      <router-link to="/News">Условия возрата и обмена</router-link>
      <router-link to="/Contacts">Контакты</router-link>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style lang="sass" scoped>
  .wrapper
    width: 100%
    height: 80px
    display: flex
    justify-content: center
    align-items: center
    box-shadow: 0 0 15px 1px
    position: fixed
    z-index: 1000000
    background-color: #fff
    top: 0
    left: 0
    nav
      width: 90%
      display: flex
      justify-content: space-evenly
      align-items: center
      a
        text-decoration: none
        color: black
        font-size: 1.5rem
        font-family: sans-serif
        position: relative
        &::after
          content: ''
          position: absolute
          left: 0
          bottom: 0
          width: 0
          height: 1px
          background-color: #222
          transition: width .5s
        &:hover::after
          width: 100%
</style>