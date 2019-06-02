<template>
  <div id="works" class="topics">
    <h1 class="section_title">Works</h1>
    <ion-icon name="logo-github" v-b-tooltip.hover title="Github" v-on:click="openUrl('https://github.com/tessai9')"></ion-icon>
    <ion-icon name="create" v-b-tooltip.hover title="Blog" v-on:click="openUrl('http://blog.livedoor.jp/tessai99/')"></ion-icon>
    <ion-icon name="people" v-b-tooltip.hover title="三宮.dev" v-on:click="openUrl('https://kobe-sannomiya-dev.connpass.com/')"></ion-icon>
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
