<template>
<div class="l-hero">
  <div class="c-container">
    <div class="img">
    <img src="~assets/images/hero/hero_logo.svg" class="p_herologo">
    </div>
    <div class="l-hero_text">
      <p>2019</p>
      <h2><span class="day">2</span>月<span class="day">16</span>日 <span class="hi">(土)</span>  10:00-</h2>
      <h3>グランパークカンファレンス</h3>
      <h4>#laraveljpcon</h4>
    </div>
  </div>
</div>
</template>


<script>
</script>

<style lang="scss" scoped>
  @import "~/assets/scss/library/variable.scss";
  @import "~/assets/scss/library/mixin.scss";


.l-hero {

  background-image: url("~assets/images/hero/hero_fuji.svg"),url( "~assets/images/hero/hero_cloud.svg"), url("~assets/images/hero/hero_bg.svg");
  background-size: cover;

  &_text {
    color: #FFF9ED;
    text-align: left;
    font-family:YuMincho;

  }
  &_text > p{
    margin-bottom:6px;
    font-size:2.5rem;
  }

  &_text > h2{
    margin-bottom:39px;
    font-size:3rem;
  }

  &_text > h3{
    margin-bottom:48px;
    font-size:4rem;
    letter-spacing: -4px;
  }

  &_text > h4{
    padding-bottom:247px;
    font-size:2rem;
    font-family:Noto Sans CJK JP;
  }

}

  .day{
    font-size:5rem;
  }
  .hi{
    font-size:4rem;
  }

  .img{
    width:100%;
    text-align: left;
    display: inline-block;
  }

  .p_herologo{
    display: inline-block;
    margin-left:70px;
    max-width:310px;
    padding-top:82px;
    padding-bottom: 43px;
  }




</style>

