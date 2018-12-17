<template>
  <div class="p-about">
    <div class="bg_deco">
      <img src="~/assets/images/about/about_left.png" class="bg_cloudLerf">
      <img src="~/assets/images/about/about_right.png" class="bg_cloudRight">
      <div class="c-container">
        <h2 class="title">
          Laravel JP conferene
        </h2>
        <span class="subTitle">ABOUT</span>
        <p class="description">
          Laravel JP Conferenceは PHPのフレームワークであるLaravelをメインテーマとした技術カンファレンスです。「Laravel JP」を冠したイベントとしては日本初開催となります。<br><br>
          <br>
          Laravelとは<br>
          2011年6月に初版が公開されたPHPによるオープンソースなWebアプリケーションフレームワーク。PHPのフレームワークの中でもGithub stars数は一番多く、Google Trendsによる人気の動向でも日本でもっとも注目を集めています。(2018年9月現在)<br><br>
          <br>
          本イベントでは主に一般公募から参加していただくスピーカーによるトークセッションと、スポンサー様から参加していただくスピーカーのトークセッション他、懇親会や参加者同士で意見交換などができる場の提供を予定しています。<br><br>
        </p>
        <div class="parent">
        </div>
        <div class="text">

        </div>
      <div class="box">
      </div>
    </div>
    </div>
  </div>
</template>

<script>
</script>

<style lang="scss" scoped>
  @import "~/assets/scss/common.scss";

  .p-about {
    @include space_section;

    background-color: #FFFCF5;

    .bg_deco {
      margin: 0 auto;
      width: 100%;
      position: relative;

      @include media_desktop {
        max-width: 2500px;
      }
    }

    .bg_cloudLerf{
      width: 20vw;
      min-width: 300px;
      max-width: 500px;
      position: absolute;
      left: 0;
      opacity: .9;
      @include media_desktop {
        opacity: 1;
      }

    }

    .bg_cloudRight {
      width: 20vw;
      min-width: 300px;
      max-width: 500px;
      position: absolute;
      bottom: 50px;
      right: 0;
      opacity: .9;

      @include media_desktop {
        bottom: -20px;
        opacity: 1;
      }
    }

    .c-container {
      position: relative;
    }

    .title {
      @include typo_sectionTitleEn;
    }
    .subTitle {
      @include typo_sectionSubTitleEn;
      top: -10rem;
    }

    .description {
      max-width: 750px;
      text-align: left;
      font-size: 1.8rem;
      color: $clr_fontBase;
      position: relative;
      z-index: 10;
    }
  }

</style>
