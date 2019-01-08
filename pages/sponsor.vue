<template>
  <div class="sponsor">
    <div class="bg_tex">
      <div class="bg_deco">
        <div class="bg_fuji"></div>
          <div class="c-container">
            <div class="info">
              <p>aaaaa</p>
            </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'sponsor'
  }
</script>

<style lang="scss" scoped>
  @import "~/assets/scss/common.scss";

  .sponsor {
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
  }

  .sponsor-box {
    width: 100%;
    height: 500px;
    background: #f8f7f2;
    @include media_desktop {
      width: 500px;
      margin: 0 auto;
    }
  }
</style>