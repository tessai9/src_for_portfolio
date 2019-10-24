<template>
  <section>
    <div id="works" class="topics">
      <h1 class="section_title">Works</h1>
      <ion-icon name="logo-github" class="icon" v-b-tooltip.hover title="Github" v-on:click="openUrl('https://github.com/tessai9')"></ion-icon>
      <ion-icon name="create" class="icon" v-b-tooltip.hover title="Blog" v-on:click="openUrl('http://tesao.work/')"></ion-icon>
      <ion-icon name="people" class="icon" v-b-tooltip.hover title="三宮.dev" v-on:click="openUrl('https://kobe-sannomiya-dev.connpass.com/')"></ion-icon>
      <ion-icon name="megaphone" class="icon" v-b-tooltip.hover title="webサービス：有言実GO" v-on:click="openUrl('https://www.yugenjigo.work/')"></ion-icon>
    </div>
  </section>
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

<style>
.icon {
  font-size: 50px;
}

.icon:hover {
  transform: scale(1.5);
}
</style>
