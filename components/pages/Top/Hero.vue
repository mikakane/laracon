<template>
<div class="p-hero">
  <div class="bg_tex">
    <div class="bg_deco">
      <div class="bg_fuji"></div>
      <div class="c-container">
        <h1 class="logo">
          <img src="~assets/images/hero/hero_logo.svg" class="p_herologo" alt="Laravel JP Conference 2019">
        </h1>
        <div class="info">
          <p class="year">2019年</p>
          <p class="date"><span class="month">2</span>月<span class="day">16</span>日 <span class="week">(土)</span>&nbsp;10:00-</p>
          <p class="location">グランパークカンファレンス</p>
          <a class="tw_hashtag" href="https://twitter.com/hashtag/laraveljpcon" target="_blank"><i class="icon fab fa-twitter"></i>#laraveljpcon</a>
        </div>
      </div>
    </div>
  </div>
</div>
</template>


<script>
</script>

<style lang="scss" scoped>
  @import "~/assets/scss/common.scss";

.p-hero {
  background: #ff554c;
  background: -moz-linear-gradient(top, #ff554c 0%, #a08383 100%);
  background: -webkit-linear-gradient(top, #ff554c 0%,#a08383 100%);
  background: linear-gradient(to bottom, #ff554c 0%,#a08383 100%);
  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#ff554c', endColorstr='#a08383',GradientType=0 );
  position: relative;
  overflow: hidden;

  .bg_tex {
    background-image: url("~assets/images/hero/hero_tex.svg");
    background-size: cover;
  }

  .bg_deco {
    display: inline-block;
    margin: 0 auto;
    width: 210vw;
    max-width: 1920px;
    min-height: 540px;
    background-size: contain;
    background-image: url( "~assets/images/hero/hero_cloud.svg");
    background-repeat: no-repeat;

    @include media_desktop {
      width: 100%;
      min-height: 900px;
      background-size: cover;
    }
  }

  .bg_fuji {
    width: 300vw;
    max-width: 1000px;
    display: inline-block;
    background-image: url("~assets/images/hero/hero_fujiyama.png");
    background-repeat: no-repeat;
    background-size: cover;
    position: absolute;
    left: 52%;
    bottom: 0;
    transform: translateX(-43%);
    @include media_desktop {
      width: 100vw;
      min-width: 1880px;
    }

    &::after {
      display: inline-block;
      content: "";
      padding-top: 42%;
    }

  }
  .c-container {
  }


  .logo {
    display: inline-block;
    margin-top: 40px;
    margin-bottom: 50px;
    width: 210px;
    height: 210px;
    transform: translateX(20%);

    @include media_desktop {
      display: inline-block;
      margin-top: 60px;
      margin-bottom: 35px;
      width: 310px;
      height: 310px;
      transform: translateX(90px);
    }
  }
  :-webkit-any(article,aside,nav,section) h1 {
    margin-block-start: 0;
    margin-block-end: 0;
  }

  .info {
    display: block;
    width: 100%;
    font-family: "游明朝体", "Yu Mincho", YuMincho, "ヒラギノ明朝 Pro", "Hiragino Mincho Pro", "MS P明朝", "MS PMincho", serif;
    font-size: 1.8rem;
    color: #FFF9ED;
    transform: translateX(20px);

    @include media_desktop {
      font-size: 2.5rem;
      transform: translateX(30px);
    }
  }
  .year {
    margin-bottom: .1em;
  }
  .date {
    font-size: 1.8rem;
    letter-spacing: 2px;
    @include media_desktop {
      font-size: 2.5rem;
    }
  }
  .month{
    font-size: 3rem;
    @include media_desktop{
      font-size: 5rem;
    }
  }
  .day{
    font-size: 3rem;
    @include media_desktop{
      font-size: 5rem;
    }
  }
  .week{
    font-size: 2rem;
    @include media_desktop{
      font-size: 4rem;
    }
  }
  .location{
    margin-bottom: 20px;
    font-size: 1.8rem;
    @include media_desktop{
      font-size: 3rem;
    }
  }
  .tw_hashtag {
    font-family: "Yu Gothic Medium", YuGothic, "Yu Gothic","ヒラギノ角ゴ Pro", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo, "ＭＳ Ｐゴシック", "MS PGothic", sans-serif;
    letter-spacing: 2px;
    color: #FFF9ED;
    text-decoration: underline;

    .icon {
      display: inline-block;
      margin-right: .4em;
      font-size: 1.2em;
      vertical-align: -3px;
    }

  }


}



</style>

