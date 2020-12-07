<template>
  <div id="app">
    <TheHeader />
    <router-view/>
  </div>
</template>

<script>
import TheHeader from '@/components/Header.vue'

export default {
  name: 'App',
  components: {
    TheHeader
  }
}
</script>

<style lang="sass">
#app
  font-family: Avenir, Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
html
  font-size: 14px
body
  margin: 0
</style>
