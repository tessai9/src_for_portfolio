<template>
  <div>
    <h1 id="header_title">I am Tetsunari Sumiyoshi</h1>
    <hr>
    <Profile></Profile>
    <Works></Works>
    <ContactMe></ContactMe>
  </div>
</template>

<script>
import Profile    from '@/components/Profile'
import ContactMe  from '@/components/ContactMe'
import Works      from '@/components/Works'

export default {
  name: 'Home',
  components: {
    Profile,
    ContactMe,
    Works
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
