<template>
  <div id="contact" class="topics">
    <h1 class="section_title">Contact me</h1>
    <ion-icon name="mail" v-b-tooltip.hover title="Send a mail" v-on:click="openMailer('shimeji9@gmail.com')"></ion-icon>
  </div>
</template>

<script>
export default {
  name: 'ContactMe',
  methods: {
    openMailer: function(address) {
      let url = "mailto:" + address
      window.location.href = url
    },
    openUrl: function(url) {
      window.open(url, '_blank')
    }
  }
}
</script>
