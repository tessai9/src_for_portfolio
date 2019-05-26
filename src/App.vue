<template>
  <div id="app" :style="{ 'background-image': 'url(' + imageSrc + ')' }">
    <PageHeader></PageHeader>
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
      imageSrc: require("@/assets/OI000001.png")
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
  height: 100vh;
}
</style>
