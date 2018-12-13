<template>
  <div class="l-about">
    <div class="parent">
      <img src="~assets/images/about/about_left.png" class="c-logo1">
      <img src="~assets/images/about/about_right.png" class="c-logo2">
    </div>
    <div class="c-container">
      <div class="parent">
      <img src="~assets/images/about/about_title.png" class="c-abouttitle">
      </div>
    <div class="title">
      Laracl JP conferene
    </div>
      <div class="text">
        <p class="text">
          Laravel JP Conferenceは PHPのフレームワークであるLaravelをメインテーマとした技術カンファレンスです。「Laravel JP」を冠したイベントとしては日本初開催となります。<br><br>
          <br>
          Laravelとは<br>
          2011年6月に初版が公開されたPHPによるオープンソースなWebアプリケーションフレームワーク。PHPのフレームワークの中でもGithub stars数は一番多く、Google Trendsによる人気の動向でも日本でもっとも注目を集めています。(2018年9月現在)<br><br>
          <br>
          本イベントでは主に一般公募から参加していただくスピーカーによるトークセッションと、スポンサー様から参加していただくスピーカーのトークセッション他、懇親会や参加者同士で意見交換などができる場の提供を予定しています。<br><br>
        </p>
      </div>
    <div class="box">
    </div>
  </div>
  </div>
</template>

<script>
</script>

<style lang="scss" scoped>
  @import "~/assets/scss/library/variable.scss";
  @import "~/assets/scss/library/mixin.scss";



  .l-about{
    background-color: #FFFCF5;
  }

  .title {
    color: #64547B;
    font-size:4rem;
    font-family: playfair-display;
    font-weight: bold;
    text-align:left;
    padding-top:7rem;
    padding-bottom:5rem;
    position: relative;
    z-index:99999;
  }

  .text {
    color: #64547B;
    text-align: left;
    max-width:750px;
    font-size: 1.7rem;
    padding-bottom: 5rem;
    position: relative;
    z-index:99999;
  }

  .c-logo1 {
    position: absolute;
    max-width: 640px;
    top: 100px;
    left:0px;
    max-width: 100%;
    @include desktop{
    position: absolute;
    max-width: 640px;
    top: 100px;
    left:0px;
    }
    }

  .c-logo2 {
    position: absolute;
    max-width: 640px;
    top: 350px;
    right:0px;
  }

  .c-abouttitle {
    position: absolute;
    max-height: 390px;
    top: -70px;
    right:0px;
    opacity: 0;
    @include desktop{
      position: absolute;
      max-height: 390px;
      top: -70px;
      right:0px;
      opacity: 100;
    }

  }

  .parent{
    position: relative;
    z-index:99;
  }


</style>
