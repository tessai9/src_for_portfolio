<template>
  <div id="contact" class="topics">
    <h1>Contact me</h1>
    <ion-icon name="logo-google" v-on:click="openMailer('shimeji9@gmail.com')"></ion-icon>
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
