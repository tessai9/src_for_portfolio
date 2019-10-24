<template>
  <section>
    <div id="profile" class="topics container">
      <h1 class="center section_title">Profile</h1>
      <b-container fluid class="text-center">
        <b-row>
          <b-col lg="2"></b-col>
          <b-col lg="2">
            <b-img class="profile_img" :src="profileImg" rounded="circle"></b-img>
          </b-col>
          <b-col class="profile_text" style="display: block;">
            <p class="text-left">
              兵庫県在住エンジニアの住吉哲斉です<br>
              自社サービス系からSES系に転職し、受託開発をしています<br>
              言語はPHP、Javascript、C++で業務経験があり、趣味でいろいろ勉強してます<br>
              勉強したことなどはブログやGitHubにて公開していますので興味があれば是非見てください
            </p>
            <p class="text-left">
              また、月一ペースで活動するエンジニアコミュニティ三宮.devの運営をしています<br>
              connpassでイベント情報を公開しているのでこちらも是非ご参加ください！
            </p>
          </b-col>
        </b-row>
      </b-container>
      <h1 class="center section_title">Skills</h1>
      <b-container>
        <b-img fluid class="skill_img" :src="skillImg.ruby"></b-img>
        <b-img fluid class="skill_img" :src="skillImg.rails"></b-img>
        <b-img fluid class="skill_img" :src="skillImg.vue"></b-img>
        <b-img fluid class="skill_img" :src="skillImg.php"></b-img>
        <b-img fluid class="skill_img" :src="skillImg.frontend"></b-img>
        <b-img fluid class="skill_img" :src="skillImg.postgresql"></b-img>
        <b-img fluid class="skill_img" :src="skillImg.docker"></b-img>
      </b-container>
    </div>
  </section>
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
  .profile_img {
    margin-right: 10px;
  }
  .skill_img {
    margin: 5px;
  }
  .profile_text {
    font-size: 1rem;
  }
</style>
