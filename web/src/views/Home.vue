<template>
  <div class="wrapper">
    <Carousel :carouselData="carouselData" :interval="5000" class="carousel" />
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
    height: calc(100vh - 80px)
    margin-top: 80px
</style>