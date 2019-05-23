<template>
  <div>
    <h1 id="header_title">I am Tetsunari Sumiyoshi</h1>
    <hr>
    <profile></profile>
    <works></works>
    <contactme></contactme>
  </div>
</template>

<script>
import profile    from '@/components/Profile.vue'
import contactme  from '@/components/ContactMe.vue'
import works      from '@/components/Works.vue'

export default {
  components: {
    profile,
    contactme,
    works
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Alfa+Slab+One&display=swap');

#header_title {
  font-family: 'Alfa Slab One', cursive;
  color: #fff;
  font-size: 70px;
}

.topics {
  color: #fff;
  font-size: 50px;
}

hr {
  background-color: #fff;
}
</style>
