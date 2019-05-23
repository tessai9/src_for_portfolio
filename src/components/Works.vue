<template>
  <div id="works" class="topics">
    <h1>Works</h1>
    <ion-icon name="logo-github" v-on:click="openUrl('https://github.com/tessai9')"></ion-icon>
    <ion-icon name="create" v-on:click="openUrl('http://blog.livedoor.jp/tessai99/')"></ion-icon>
  </div>
</template>

<script>
export default {
  name: 'Works',
  methods: {
    openUrl: function(url) {
      window.open(url, '_blank')
    }
  }
}
</script>
