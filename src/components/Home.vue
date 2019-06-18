<template>
  <div>
    <h1 id="header_title">I am Tetsunari Sumiyoshi</h1>
    <hr>
    <b-container fluid>
      <Profile></Profile>
    </b-container>
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
@import url('https://fonts.googleapis.com/css?family=Audiowide&display=swap');


#header_title {
  padding-top: 3px;
  font-family: 'Alfa Slab One', cursive;
  color: #fff;
  font-size: 6vw;
}

.topics {
  color: #fff;
  margin-top: 20px;
}

.section_title {
  font-family: 'Audiowide', cursive;
}

.icon {
  font-size: 50px;
}

hr {
  background-color: #fff;
}
</style>
