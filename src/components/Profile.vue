<template>
    <section id="profile" class="profile-section bg-light">
  <div class="container">
    <div class="row section-title-wrapper">
      <h1 class="col-12">Profile</h1>
    </div>
    <div class="row">
      <div class="col-md-4 profile-img-wrapper">
        <img v-bind:src="profileImg">
      </div>
      <p class="col-md-8">
        アクセスしていただきありがとうございます。<br>
        2020年4月よりプログラマになりました、たかみんと申します。歳は23です。
        <br><br>
        新卒ではITベンダーにバックエンドエンジニアとして入社しました。言語はJavaを使用しています。<br>
        大学では英文学を専攻しており、おかげで英語の文献に全く忌避感がありません。<br><br>
        バックエンドで開発しているうちにインフラに興味を持ったため、現在は社内でAWSの構築とバックエンドアプリの開発を行っています（フロントも多少Vueを触ります）。<br><br>
        バックエンドとインフラがとても強く、フロントも最低限こなせるエンジニアが現在の目標です。<br>
        20代はバリバリコードを書いていきたいです。
      </p>
    </div>
  </div>
</section>
</template>

<script>
export default {
    name: 'Profile',
    data() {
        return {
            profileImg: '/cup2.png'
        }
    }
}
</script>

<style scoped>
.profile-img-wrapper{
  display: flex;
  justify-content: center;
  align-items: center;
}

.profile-img-wrapper img{
  padding: 10px;
  max-width: 80%;
  height:auto;
  border-radius: 50%;
}
</style>