<template>
  <section class="p-sponsor">
    <div class="c-container">
      <h3 class="title">Sponsor</h3>

      <div class="sponsorGold">
        <div class="sponsorGold_rank">GOLD</div>
        <div class="sponsorList-gold">
          <div class="sponsorList-gold_item" v-for="(val,key) in sponsors.GOLD.sponsors" :key="key">
            <div class="sponsorList-gold_logo" :title="val.name"></div>
            <router-link to="#" class="sponsorList-gold_button">
              紹介ページへ
            </router-link>
          </div>
        </div>
      </div>
      <div class="sponsorSilver">
        <div class="sponsorSilver_rank">SILVER</div>
        <div class="sponsorList-silver">
          <div class="sponsorList-silver_item" v-for="(val,key) in sponsors.SILVER.sponsors" :key="key">
          <div class="sponsorList-silver_logo" :title="val.name"></div>
          <router-link to="#" class="sponsorList-silver_button">
              紹介ページへ
          </router-link>
          </div>
        </div>
      </div>
      <div class="sponsorBronze">
        <div class="sponsorBronze_rank">BRONZE</div>
        <div class="sponsorList-bronze">
          <div class="sponsorList-bronze_item" v-for="(val,key) in sponsors.BRONZE.sponsors" :key="key">
            <div class="sponsorList-bronze_logo" :title="val.name"></div>
            <router-link to="#" class="sponsorList-bronze_button">
              紹介ページへ
            </router-link>
          </div>
        </div>
      </div>
      <div class="sponsorOthers">

        <div class="sponsorList-others">
          <div class="sponsorList-others_item" v-for="(val,key) in sponsors.LUNCH.sponsors" :key="key">
            <div class="sponsorOthers_rank">LUNCH</div>
            <div class="sponsorList-others_logo" :title="val.name"></div>
            <router-link to="#" class="sponsorList-others_button">
              紹介ページへ
            </router-link>
          </div>
          <div class="sponsorList-others_item" v-for="(val,key) in sponsors.DRINK.sponsors" :key="key">
            <div class="sponsorOthers_rank">DRINK</div>
            <div class="sponsorList-others_logo" :title="val.name"></div>
            <router-link to="#" class="sponsorList-others_button">
              紹介ページへ
            </router-link>
          </div>
          <div class="sponsorList-others_item" v-for="(val,key) in sponsors.DRINK.sponsors" :key="key">
            <div class="sponsorOthers_rank">ECOBAG</div>
            <div class="sponsorList-others_logo" :title="val.name"></div>
            <router-link to="#" class="sponsorList-others_button">
              紹介ページへ
            </router-link>
          </div>
          <div class="sponsorList-others_item" v-for="(val,key) in sponsors.DESIGN.sponsors" :key="key">
            <div class="sponsorOthers_rank">DESIGN</div>
            <div class="sponsorList-others_logo" :title="val.name"></div>
            <router-link to="#" class="sponsorList-others_button">
              紹介ページへ
            </router-link>
          </div>
          <div class="sponsorList-others_item" v-for="(val,key) in sponsors.SUPPORT.sponsors" :key="key">
            <div class="sponsorOthers_rank">SUPPORT</div>
            <div class="sponsorList-others_logo" :title="val.name"></div>
            <router-link to="#" class="sponsorList-others_button">
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
    props: {
      sponsors: {
        type: Object,
        required: true
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import "~/assets/scss/common.scss";

  // common mixin
  @mixin space_rank {
    margin-bottom: 50px;
    @include media_desktop {
      margin-bottom: 80px;
    }
  }

  @mixin rank {
    display: block;
    margin-bottom: .5em;
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
    padding: 10px 10px;
    font-size: 1.2rem;
    color: white;
    background: $clr_btn;
    text-align: center;
    position: relative;

    @include media_desktop {
      padding: 20px 10px;
      font-size: 1.4rem;
    }

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
      right: 5px;
      top: 50%;
      transform: translateY(-50%);

      @include media_desktop {
        right: 10px;
      }

    }
  }

  // section
  .p-sponsor {
    @include space_section;

    .title {
      @include typo_sectionTitleEn
    }

    background-color: #FAEAE6;


    // sponsor GOLD
    .sponsorGold {
      @include space_rank;
    }
    .sponsorGold_rank {
      @include rank;
    }

    .sponsorList-gold {
      display: flex;
      flex-wrap: wrap;
      justify-content: flex-start;
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

    // sponsor SILVER
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
      justify-content: flex-start;
      max-width: 768px;
      width: 100%;
    }
    .sponsorList-silver_item{
      margin-right: 20px;
      margin-bottom: 20px;
      width: calc((100% - 20px) / 2);

      &:nth-of-type(2n) {
        margin-right: 0;
      }
      &:nth-of-type(5) {
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
      }
    }
    .sponsorList-silver_logo{
      @include logo;
    }
    .sponsorList-silver_button{
      @include button;
    }

    // sponsor BRONZE
    .sponsorBronze {
      @include space_rank;
      text-align: center;
    }
    .sponsorBronze_rank {
      @include rank;
    }

    .sponsorList-bronze{
      display: inline-flex;
      flex-wrap: wrap;
      justify-content: flex-start;
      width: 100%;
    }
    .sponsorList-bronze_item{
      margin-right: 10px;
      margin-bottom: 20px;
      width: calc((100% - 20px) / 3);
      &:nth-of-type(3n) {
        margin-right: 0;
      }

      @include media_desktop {
        margin-right: 30px;
        margin-bottom: 30px;
        width: calc((100% - 120px) / 5);

        &:nth-of-type(3n) {
          margin-right: 30px;
        }

        &:nth-of-type(5n) {
          margin-right: 0;
        }
      }
    }
    .sponsorList-bronze_logo{
      @include logo;
    }
    .sponsorList-bronze_button{
      @include button;
    }

    // sponsor OHTERS

    .sponsorOthers {
      @include space_rank;
      text-align: center;
    }
    .sponsorOthers_rank {
      @include rank;
    }

    .sponsorList-others{
      display: inline-flex;
      flex-wrap: wrap;
      justify-content: flex-start;
      max-width: 768px;
      width: 100%
    }
    .sponsorList-others_item{
      margin-right: 20px;
      margin-bottom: 20px;
      width: calc((100% - 20px) / 2);

      &:nth-of-type(2n) {
        margin-right: 0;
      }
      &:nth-of-type(5) {
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

      }
    }
    .sponsorList-others_logo{
      @include logo;
    }
    .sponsorList-others_button{
      @include button;
    }


  }

</style>
