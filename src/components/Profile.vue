<template>
  <div id="profile" class="topics container">
    <b-row>
      <b-col class="float-right">
        <h1 class="center section_title">Profile</h1>
        <b-img class="profile_img" :src="profileImg" rounded="circle"></b-img>
        <p class="contents_text text-left">
          今年（2019年）で社会人4年目になる兵庫県在住のエンジニア<br>
          LAPP製の業務システム会社へ2016年に新卒で入社し、2年半ほど保守／開発を担当したのちSES会社へ転職。<br>
          現在、常駐先の現場にてC++ ＋ DB2製の業務システムの保守／開発を担当。<br>
        </p>
        <p class="contents_text text-left">
          別途、三宮で活動するコミュニティ 三宮.dev を運営中。<br>
          月一ペースで勉強会を開催。
        </p>
      </b-col>
      <b-col>
          <h1 class="center section_title">Skills</h1>
          <img class="skill_img" :src="skillImg.ruby">
          <img class="skill_img" :src="skillImg.rails">
          <img class="skill_img" :src="skillImg.vue">
          <img class="skill_img" :src="skillImg.php">
          <img class="skill_img" :src="skillImg.frontend">
          <img class="skill_img" :src="skillImg.postgresql">
          <img class="skill_img" :src="skillImg.docker">
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  name: 'Profile',
  data () {
    return {
      profileImg: require("@/assets/52a6dde5_prof.png"),
      skillImg: {
        ruby: require("@/assets/ruby.png"),
        rails: require("@/assets/rails.png"),
        vue: require("@/assets/vue.png"),
        docker: require("@/assets/docker.png"),
        frontend: require("@/assets/frontend.png"),
        postgresql: require("@/assets/postgresql.png"),
        php: require("@/assets/php.png")
      }
    }
  }
}
</script>

<style>
  .contents_text {
    font-size: 15px;
  }

  .profile_img {
    height: 130px;
  }

  .skill_img {
    height: 70px;
    margin: 5px;
  }
</style>
