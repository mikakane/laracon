<template>
  <section class="p-sponsor">
    <div class="c-container">
      <h3 class="title">Sponsor</h3>

      <div class="sponsorGold">
        <div class="sponsorGold_title">GOLD</div>
        <div class="sponsorList-gold">
          <div class="sponsorList-gold_item" v-for="(val,key) in [1,2,3]" :key="key">
            <div class="sponsorList-gold_logo"></div>
            <router-link to="#" class="sponsorList-gold_button">
              紹介ページを見る
            </router-link>
          </div>
        </div>
      </div>
      <i></i>

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

  .p-sponsor {
    @include space_section;

    .title {
      @include typo_sectionTitleEn
    }

    background-color:#FAEAE6;
    .sponsorGold {

    }

    .sponsorList-gold {
      display: flex;
      flex-wrap: wrap;
      justify-content: flex-start;
    }
    .sponsorGold_title {
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

    .sponsorList-gold{

    }

    .sponsorList-gold_item {
      margin-bottom: 30px;
      width: 100%;

      @include media_desktop {
        margin-right: 30px;
        width: calc((100% - 60px) / 3 );

        &:nth-of-type(3n) {
          margin-right: 0;
        }
      }

    }
    .sponsorList-gold_logo {
      width: 100%;
      background-image: url("https://via.placeholder.com/600x600");
      background-position: center;
      background-repeat: no-repeat;
      background-size: contain;
      background-color: white;

      &::after {
        display:  block;
        content: "";
        padding-top: 100%;
      }
    }
    .sponsorList-gold_button {
      display: block;
      padding: 20px 10px;
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

        @include media_desktop {
          font-size: 1.7em;
        }
      }

    }

    &_heading {
        color: #64547B;
        font-size:4rem;
        font-family: playfair-display;
        font-weight: bold;
        text-align:left;
        padding-top:7rem;
    }

    &_read {
    }

    .title {
    }
    .row {
      justify-content: flex-start;
    }
    .btn {
      display: block;
      width: 100%;
      padding: 1em 0;
      font-size: 1.3rem;
      font-weight: bold;
      color: white;
      text-decoration: none;
      background: #E36F65;
      cursor: pointer;
      transition: opacity .3s;

      @include media_desktop {
        font-size: 1.8rem;
        font-weight: normal;
      }

      :hover {
        opacity: .9;
        transition: opacity .3s;
      }

      i {
        margin-left: .5em;
      }
    }


    .list {
      box-sizing: border-box;
      text-align: center;

    }
    .listItem {
      margin-bottom: 40px;
      box-sizing: border-box;
      padding: 40px 0 0;
      text-align: center;
      background: white;
      @include media_desktop {
        padding: 50px 0 0;
      }

      .inner {
        width: 100%;
        margin: 0 auto 30px;
        padding: 0 30px;
        display: inline-block;
        text-align: left;
        box-sizing: border-box;

        @include media_desktop {
          margin: 0 auto 40px;
        }
      }
    }

    &_platinum {
      margin-bottom: 30px;
      @include media_desktop {
        margin-bottom: 60px;
      }

      @include media_desktop {

      }
      .row {
        justify-content: center;
      }
      .listItem {
        .inner {
          max-width: 660px;
        }
        .thumb {
          display: inline-block;
          margin-bottom: 15px;
          width: 100%;
          max-width: 600px;
          background-image: url("http://placehold.it/600x480");
          background-repeat: no-repeat;
          background-size: contain;
          background-position: center;

          &::before {
            content: "";
            display: block;
            padding-top: 80%;
          }
        }

        .description {
          display: inline-block;
          width: 100%;
          box-sizing: border-box;

          @include media_desktop {
            max-width: 600px;
          }
        }

      }
    }

    &_gold {
      margin-bottom: 30px;
      @include media_desktop {
        margin-bottom: 60px;
      }
      .list {

      }
      .listItem {
        .inner {
          max-width: 100%;
          @include media_desktop {
            max-width: 360px;
          }
        }
        .thumb {
          display: block;
          margin: 0 auto;
          margin-bottom: 15px;
          width: 100%;
          max-width: 200px;
          background-image: url("http://placehold.it/300x240");
          background-repeat: no-repeat;
          background-size: contain;
          background-position: center;

          @include media_desktop {
            max-width: 300px;
          }

          &::before {
            content: "";
            display: block;
            padding-top: 80%;
          }
        }
      }
    }

    &_silver {
      margin-bottom: 30px;
      @include media_desktop {
        margin-bottom: 60px;
      }

      .list {
        box-sizing: border-box;
        width: 50%;
        padding-right: 10px;
        padding-left: 10px;
      }

      .listItem {
        margin-bottom: 20px;
        padding-top: 30px;

        @include media_desktop {
          margin-bottom: 30px;
        }

        .inner {
          margin-bottom: 20px;
          width: 100%;
          padding: 0 20px;
          @include media_desktop {
            max-width: 260px;
          }
        }
        .thumb {
          display: block;
          margin: 0 auto;
          width: 100%;
          max-width: 160px;
          background-image: url("http://placehold.it/200x160");
          background-repeat: no-repeat;
          background-size: contain;
          background-position: center;

          @include media_desktop {
            max-width: 200px;
          }

          &::before {
            content: "";
            display: block;
            padding-top: 80%;
          }
        }
      }
    }
    &_bronze {
      margin-bottom: 30px;
      @include media_desktop {
        margin-bottom: 60px;
      }

      .list {
        box-sizing: border-box;
        width: calc( 100% / 3 );
        padding-right: 5px;
        padding-left: 5px;

        @include media_desktop {
          padding-right: 15px;
          padding-left: 15px;
        }

      }

      .listItem {
        margin-bottom: 10px;
        padding-top: 10px;
        @include media_desktop {
          margin-bottom: 30px;
          padding-top: 20px;
        }
        .inner {
          margin-bottom: 5px;
          max-width: 220px;
          text-align: center;
          padding: 0 10px;
          @include media_desktop {
            margin-bottom: 20px;
            padding: 0 20px;
          }
        }
        .thumb {
          display: block;
          margin: 0 auto;
          max-width: 160px;
          background-image: url("http://placehold.it/160x128");
          background-repeat: no-repeat;
          background-size: contain;
          background-position: center;

          &::before {
            content: "";
            display: block;
            padding-top: 80%;
          }
        }
      }
    }
  }

</style>
