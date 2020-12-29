<template>
  <div class="wrapper">
    <div class="first">@2009-2020</div>
    <div class="second">
      <div class="top-content">
        <a href="https://vk.com/">VKONTAKTE</a>
        <a href="https://facebook.com/">FACEBOOK</a>
        <a href="https://instagram.com/">INSTAGRAM</a>
        <a href="https://youtube.com/">YOUTUBE</a>
      </div>
      <div class="bottom-content">
        Политика Конфиденциальности
      </div>
    </div>
    <div class="third">
      +7 (777) 777-77-77 <br>
      СЛУЖБА ПОДДЕРЖКИ С 9 до 21
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style lang="sass" scoped>
  a
    text-decoration: none
    color: white
  .wrapper
    width: 100%
    height: 120px
    background-color: #222
    display: flex
    justify-content: space-evenly
    align-items: center
    color: white
    .first
      width: 33.33333333%
      display: flex
      justify-content: center
      align-items: center
    .second
      width: 33.33333333%
      display: flex
      flex-direction: column
      justify-content: center
      align-items: center
      height: 100%
      .top-content
        width: 100%
        display: flex
        justify-content: space-evenly
        align-items: center
        font-size: 1.2rem
      .bottom-content
        width: 100%
        display: flex
        justify-content: center
        align-items: center
        font-size: 1rem
        margin-top: 10px
    .third
      width: 33.33333333%
      display: flex
      align-items: center
      justify-content: center
</style>