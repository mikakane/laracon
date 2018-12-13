
  <template>
    <div class="l-access">
      <div class="c-container">
        <div class="parent">
          <img src="~assets/images/access/access_bg.png" class="c-logo1">
          <img src="~assets/images/access/access_title.png" class="c-logo2">
        </div>
        <div class="box">
          <iframe src="https://www.google.com/maps/embed?pb=!1m16!1m12!1m3!1d3242.349875889781!2d139.74365216567548!3d35.64375058020296!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!2m1!1z5p2x5Lqs6YO95riv5Yy66Iqd5rWmM-S4geebrjQtMSDnlLDnlLrjgrDjg6njg7Pjg5Hjg7zjgq_jgIDjg5fjg6njgrbmo5_vvJPpmo7jg7vvvJTpmo4!5e0!3m2!1sja!2sjp!4v1544585900455" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>

          <div class="access-box">
            <h3>会場とアクセス</h3>
            <div class="d">住所</div>
            <p>東京都港区芝浦3丁目4-1<br>
              田町グランパーク　プラザ棟３階・４階</p>
            <div class="d">最寄り駅からの所用時間</div>
            <p>JR田町駅（徒歩5分）<br>
              地下鉄都営浅草線 三田駅（徒歩7分）</p>
            <div class="btn">
              <p class="btn_text">GoogleMapで開く</p>
            </div>
          </div>

      </div>
      </div>
    </div>
  </template>


<script>
</script>

<style lang="scss" scoped>
  @import "~/assets/scss/library/variable.scss";
  @import "~/assets/scss/library/mixin.scss";




  iframe{
    width: 100%;
    height:440px;
    z-index: 990;
    padding-top:50px;
    float: right;
    @include desktop {
      width: 75%;
    }
    }


  .access-box{
    max-width:450px;
    background-color:#786A7D;
    z-index: 999;
    padding:30px;


    position: absolute;
    top: 380px;
    float: left;
  }

  .access-box> h3{
    color:#fff;
    font-size:3rem;
    font-weight: bold;
    padding-top:20px;
    margin-bottom: 40px;
  }

  .access-box> p{
    color:#fff;
    font-size:1.6rem;
    text-align: left;
    margin-bottom: 35px;
  }

  .d{
    color: #ffffff;
    font-size:1.7rem;
    text-align: left;
  }

  .btn{
    width: 100%;
    background-color:#E36F65;
  }

  .btn_text{
    color:#fff;
    font-size:1.8rem;
    font-weight: bold;
    margin:20px 0;
  }


  .c-logo1 {
    position: absolute;
    max-height: 710px;
    max-width:100%;
    top: 250px;
    right:0px;
    opacity: 0;
    @include desktop{
      opacity: 100;
    }

  }
  .c-logo2 {
    position: absolute;
    max-height: 450px;
    top: -45px;
    left:0px;
    z-index: 1000;
    opacity: 0;
    @include desktop{
      opacity: 100;
    }
  }


  .parent{
    position: relative;
  }

  .box{
    position: relative;
    padding-bottom: 900px;
  }

</style>
