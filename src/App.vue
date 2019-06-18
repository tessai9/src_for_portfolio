<template>
  <div id="app" :style="{ 'background-image': 'url(' + backgroundImageSrc + ')' }">
    <router-view/>
  </div>
</template>

<script>
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
import PageHeader from '@/components/PageHeader.vue'

export default {
  name: 'App',
  data () {
    return {
      backgroundImageSrc: require("@/assets/OI000001.png")
    }
  },
  components: {
    PageHeader
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: no-repeat center;
  min-height: 100vh;
  width: 100vw;
}
</style>
