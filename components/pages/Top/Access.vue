
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
          <div class="access-box">
            <h2 class="title">
              会場とアクセス
            </h2>
            <dl>
              <dt><i class="fas fa-map-marker-alt"></i>住所</dt>
              <dd>東京都港区芝浦3丁目4-1<br>
                田町グランパーク　プラザ棟３階・４階</dd>
            </dl>
            <dl>
              <dt><i class="fas fa-subway"></i>最寄り駅からの所用時間</dt>
              <dd>JR田町駅（徒歩5分</dd>
              <dd>地下鉄都営浅草線 三田駅（徒歩7分）</dd>
            </dl>
            <a class="btn" href="https://goo.gl/maps/jjKtmTcffSm" target="_blank">
              GoogleMapで開く
            </a>
          </div>
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

    .bg_deco {
      position: relative;
    }
    .bgImage {
      display: none;
      position: absolute;
      right: 0;
      bottom: -50px;
      @include media_desktop{
        display: inline-block;
      }
    }

    .c-container {
      position: relative;
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
      height: 450px;
      position: relative;
    }
    .accessInfo {
      max-width: 450px;
      padding: 50px 30px;
      color: white;
      background-color: #786A7D;
      position: relative;
      left: 0;
      top: -25px;
      z-index: 100;
    }

  }

</style>
