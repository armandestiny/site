<template>
<div class="text">
  <div class="wrapper">
    <Carousel :carouselData="carouselData" :interval="5000" class="carousel" />
  </div>
  <br>
  <br>
  <br>
  <br>
  <br>
  <span align="center">Добро пожаловать на наш сайт</span>
  <p align="justify">
    ТОО «Новые образовательные технологии» работает с января 2016 года. Целью деятельности ТОО «Новые образовательные технологии» (ТОО НОТ) является оказание широким слоям населения и профессиональным сообществам электронных образовательных услуг в рамках <br>
    развития единой информационно-образовательной коммуникативно-обучающей среды с использованием возможностей современных ИКТ и глобальной сети Интернет. <br>
      Предметом деятельности ТОО НОТ является: <br>
      •	создание и развитие цифровой мультимедиа-индустрии как прорывного научно-технологического проекта, обеспечивающего доступ к открытому демократическому образованию в Республике Казахстан; <br>
      •	формирование единой информационно-образовательной и коммуникативно-обучающей среды; <br>
      •	организация системы профессионально-ориентированного дистанционного обучения; <br>
      •	содействие развитию рынка интеллектуальной собственности, малого и среднего бизнеса в области разработки современных ИКТ <br>
       и профессионально-ориентированного цифрового образовательного контента. <br>
</p>
<div class="contacts">
    <link rel="stylesheet" href="./style/style.css">
    <center><h5>Обратная связь</h5></center>
    <form id="form_input">
      <label for="name">Имя <span>*</span></label><br>
      <input type="text" placeholder="Введите имя" name="name" id="name"><br>
      <label for="email">Ваша почта <span>*</span></label><br>
			<input type="email" placeholder="Введите email" name="email" id="email"><br>
			<label for="message">Сообщение <span>*</span></label><br>
			<textarea placeholder="Введите ваше сообщение" name="message" id="message"></textarea><br>
			<div id="mess_send" class="btn">Отправить</div>
    </form>
  </div>
</div>  
</template>

<script>
// @ is an alias to /src
import Carousel from '@/components/Carousel.vue'

export default {
  name: 'Home',
  components: {
    Carousel
  },
  data: () => ({
    carouselData: [
      {
        id: '_' + Math.random().toString(36).substr(2, 9),
        imageName: 'logo.png'
      },
      {
        id: '_' + Math.random().toString(36).substr(2, 9),
        imageName: '1.jpg'
      },
      {
        id: '_' + Math.random().toString(36).substr(2, 9),
        imageName: '2.jpg'
      },
      {
        id: '_' + Math.random().toString(36).substr(2, 9),
        imageName: '3.jpg'
      },
      {
        id: '_' + Math.random().toString(36).substr(2, 9),
        imageName: '4.jpg'
      }
    ]
  })
}
</script>

<style lang="sass" scoped>
  .carousel
    height: calc(90vh - 80px)
    position: absolute
    top: 100%
    left: 50%
    margin-right: -50%
    transform: translate(-50%, -50%)
    margin-top: 170px
    width: 70em
  span
    width: 100%
    text-align: center
    font-size: 2.5rem
  .text
    margin-left: auto
    margin-right: auto
    width: 40em
    min-height: calc(300vh - 80px)
    font-size: 1.3rem
    text-align: center
  .contacts
    position: absolute
    top: 100%
    left: 50%
    margin-right: -50%
    transform: translate(-50%, 140%)
    margin-top: 170px
 </style>