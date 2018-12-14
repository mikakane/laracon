<template>
  <section class="p-sponsor">
    <div class="c-container">
      <h3 class="title">Sponsor</h3>

      <div class="sponsorGold">
        <div class="sponsorGold_rank">GOLD</div>
        <div class="sponsorList-gold">
          <div class="sponsorList-gold_item" v-for="(val,key) in [1,2,3]" :key="key">
            <div class="sponsorList-gold_logo"></div>
            <router-link to="#" class="sponsorList-gold_button">
              紹介ページへ
            </router-link>
          </div>
        </div>
      </div>
      <div class="sponsorSilver">
        <div class="sponsorSilver_rank">SILVER</div>
        <div class="sponsorList-silver">
          <div class="sponsorList-silver_item" v-for="(val,key) in [1,2,3,4,5]" :key="key">
          <div class="sponsorList-silver_logo"></div>
          <router-link to="#" class="sponsorList-gold_button">
              紹介ページへ
          </router-link>
          </div>
        </div>
      </div>

    </div>
  </section>
</template>

<script>

  export default  {
    components: {

    }
  }
</script>

<style lang="scss" scoped>
  @import "~/assets/scss/common.scss";

  /*mixin*/
  @mixin space_rank {
    margin-bottom: 50px;
    @include media_desktop {
      margin-bottom: 80px;
    }
  }

  @mixin rank {
    display: block;
    margin-bottom: .8em;
    font-family: 'Playfair Display', serif;
    text-transform: capitalize;
    font-size: 1.8rem;
    font-weight: normal;
    letter-spacing: 1px;
    color: $clr_fontBase;
    text-align: center;

    @include media_desktop {
      margin-bottom: 1em;
    }
  }

  @mixin logo {
    width: 100%;
    background-image: url("https://via.placeholder.com/600x600");
    background-position: center;
    background-repeat: no-repeat;
    background-size: contain;
    background-color: white;

    &::after {
      display: block;
      content: "";
      padding-top: 100%;
    }
  }

  @mixin button {
    display: block;
    padding: 20px 10px;
    font-size: 1.4rem;
    color: white;
    background: $clr_btn;
    text-align: center;
    position: relative;

    &::after {
      content: "\f054";
      display: inline-block;
      font-family: "Font Awesome 5 Free";
      font-size: 1em;
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
    }
  }

  .p-sponsor {
    @include space_section;

    .title {
      @include typo_sectionTitleEn
    }

    background-color: #FAEAE6;

    .sponsorGold {
      @include space_rank;
    }
    .sponsorGold_rank {
      @include rank;
    }

    .sponsorList-gold {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
    }

    .sponsorList-gold_item {
      margin-bottom: 30px;
      width: 100%;

      @include media_desktop {
        margin-right: 30px;
        width: calc((100% - 60px) / 3);

        &:nth-of-type(3n) {
          margin-right: 0;
        }
      }

    }
    .sponsorList-gold_logo {
      @include logo;
    }
    .sponsorList-gold_button {
      @include button;
    }

    .sponsorSilver {
      @include space_rank;
      text-align: center;
    }
    .sponsorSilver_rank {
      @include rank;
    }

    .sponsorList-silver{
      display: inline-flex;
      flex-wrap: wrap;
      justify-content: center;
      max-width: 768px;
    }
    .sponsorList-silver_item{
      margin-right: 20px;
      margin-bottom: 20px;
      width: calc((100% - 20px) / 2);

      &:nth-of-type(2n) {
        margin-right: 0;
      }

      @include media_desktop {
        margin-right: 30px;
        margin-bottom: 30px;
        width: calc((100% - 60px) / 3);

        &:nth-of-type(2n) {
          margin-right: 30px;
        }

        &:nth-of-type(3n) {
          margin-right: 0;
        }
        &:nth-of-type(5) {
          margin-right: 0;
        }
      }
    }
    .sponsorList-silver_logo{
      @include logo;
    }
    .sponsorList-silver_button{
      @include button;
    }
  }

</style>
