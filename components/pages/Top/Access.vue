
  <template>
    <section class="p-access">
      <div class="bg_deco">

      </div>
      <div class="c-container">
        <img src="~assets/images/access/access_bg.png" class="bgImage">
        <span class="subTitle">ACCESS</span>
        <div class="accessMap">
          <iframe class="googleMap" src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d6484.699717709147!2d139.743652!3d35.643751!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x60188bb398b1dd0d%3A0x29cde45fbedace6e!2z44Kw44Op44Oz44OR44O844Kv44Kr44Oz44OV44Kh44Os44Oz44K5!5e0!3m2!1sja!2sjp!4v1544782459878" frameborder="0" style="border:0" allowfullscreen></iframe>
        </div>
        <div class="accessInfo">
          <h2 class="title">
            会場とアクセス
          </h2>
          <dl class="access_dl">
            <dt class="access_dt"><i class="icon fas fa-map-marker-alt"></i>住所</dt>
            <dd class="access_dd">東京都港区芝浦3丁目4-1<br>
              田町グランパーク　プラザ棟３階・４階</dd>
          </dl>
          <dl class="access_dl">
            <dt class="access_dt"><i class="icon fas fa-subway"></i>最寄り駅からの所用時間</dt>
            <dd class="access_dd">JR田町駅（徒歩5分</dd>
            <dd class="access_dd">地下鉄都営浅草線 三田駅（徒歩7分）</dd>
          </dl>
          <a class="btn" href="https://goo.gl/maps/jjKtmTcffSm" target="_blank">
            GoogleMapで開く
          </a>
        </div>
      </div>
    </section>
  </template>


<script>
</script>

<style lang="scss" scoped>
  @import "~/assets/scss/common.scss";

  .p-access {
    @include space_section;
    padding-top: 0;

    @include media_desktop {
      padding-top: 60px;
    }

    .bg_deco {
      position: relative;
    }
    .bgImage {
      display: none;
      position: absolute;
      right: 0;
      bottom: -70px;
      @include media_desktop{
        display: inline-block;
      }
    }

    .c-container {
      position: relative;
      padding: 0;
      @include media_desktop {
        padding: 0 20px;
      }
    }

    .subTitle {
      @include typo_sectionSubTitleEn;
      top: -1.6rem;
      left: 50px;
      z-index: 200;
    }
    .accessMap {
      text-align: right;
    }
    .googleMap {
      width: 100%;
      max-width: 750px;
      height: 300px;
      position: relative;

      @include media_desktop {
        height: 450px;
      }
    }
    .accessInfo {
      width: calc(100% - 40px);
      padding: 30px 20px;
      color: white;
      background-color: #786A7D;
      position: relative;
      left: 50%;
      top: -25px;
      z-index: 100;
      transform: translateX(-50%);
      @include media_desktop {
        max-width: 450px;
        padding: 50px 30px;
        left: 0;
        transform: translateX(-50%);
      }
    }
    .title {
      @include typo_sectionTitleJa;
      text-align: center;
      color: white;
    }
    .access_dl {
      margin-bottom: 40px;
      letter-spacing: 1px;
    }
    .access_dt {
      font-size: 2rem;
      font-weight: normal;
      margin-bottom: 15px;
      .icon {
        display: inline-block;
        margin-right: .4em;
        font-size: 1.2em;
        vertical-align: -2px;
      }
    }
    .access_dd {

    }
    .btn {
      display: block;
      padding: 20px;
      color: white;
      font-size: 2rem;
      font-weight: bold;
      background: $clr_btn;
      position: relative;
      &::after {
        content: "\f35d";
        display: inline-block;
        font-family: "Font Awesome 5 Free";
        font-size: .8em;
        font-style: normal;
        font-weight: bold;
        font-variant: normal;
        text-rendering: auto;
        line-height: 1;
        color: #fff;
        position: absolute;
        right: 10px;
        top: 50%;
        transform: translateY(-50%);

        @include media_desktop {
          right: 10px;
        }

      }

    }

  }

</style>
