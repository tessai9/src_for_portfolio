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
              兵庫県在住のエンジニアの住吉哲斉です<br>
              自社サービス系からSES系に転職し、現在は客先常駐SEとして業務システムの保守／開発を担当<br>
              言語はPHP、Javascript、C++の業務経験がありますが、個人的にRubyとRustを中心に勉強中<br>
              その他、DockerやAWSなどのインフラも併せて勉強中
            </p>
            <p class="text-left">
              別途、三宮で活動するコミュニティ三宮.devを運営中<br>
              月一ペースで勉強会を開催中
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
