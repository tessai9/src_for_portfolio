<template>
  <div>
    <h1 id="header_title">I am Tetsunari Sumiyoshi</h1>
    <hr>
    <b-container fluid>
      <Profile></Profile>
    </b-container>
    <Works></Works>
    <ContactMe></ContactMe>
    <b-modal id="old_portfolio" title="ここは古いポートフォリオです">
      <p>このポートフォリオは旧版です。もう更新されていません。</p>
      <p>新しいポートフォリオは<a href="https://tessai9.github.io/portfolio_v2/">こちら</a>です。</p>
    </b-modal>
  </div>
</template>

<script>
import Profile    from '@/components/Profile'
import ContactMe  from '@/components/ContactMe'
import Works      from '@/components/Works'

export default {
  name: 'Home',
  mounted() {
this.$bvModal.show('old_portfolio')
  },
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

hr {
  background-color: #fff;
}
</style>
