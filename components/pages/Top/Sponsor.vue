<template>
  <section class="p-sponsor">
    <div class="c-container">
      <h3 class="p-sponsor_heading">Sponsor</h3>

      <div class="p-sponsor_silver">
        <div class="title">
          Silver
        </div>
        <div class="row">
          <div class="list col-sm-4">
            <div class="listItem">
              <div class="inner">
                <a href="#" ><div class="thumb"/></a>
              </div>
              <router-link
                to="/jobs"
                class="btn">広告・求人ページ<i class="fas fa-chevron-right"></i>
              </router-link>
            </div>
          </div>
          <div class="list col-sm-4">
            <div class="listItem">
              <div class="inner">
                <a href="#" ><div class="thumb"/></a>
              </div>
              <router-link
                to="/jobs"
                class="btn">広告・求人ページ<i class="fas fa-chevron-right"></i>
              </router-link>
            </div>
          </div>
          <div class="list col-sm-4">
            <div class="listItem">
              <div class="inner">
                <a href="#" ><div class="thumb"/></a>
              </div>
              <router-link
                to="/jobs"
                class="btn">広告・求人ページ<i class="fas fa-chevron-right"></i>
              </router-link>
            </div>
          </div>
          <div class="list col-sm-4">
            <div class="listItem">
              <div class="inner">
                <a href="#" ><div class="thumb"/></a>
              </div>
              <router-link
                to="/jobs"
                class="btn">広告・求人ページ<i class="fas fa-chevron-right"></i>
              </router-link>
            </div>
          </div>
        </div>
      </div>
      <div class="p-sponsor_bronze">
        <div class="title">
          Bronze
        </div>
        <div class="row">
          <div class="list col-sm-3">
            <div class="listItem">
              <div class="inner">
                <a href="#" ><div class="thumb"/></a>
              </div>
            </div>
          </div>
          <div class="list col-sm-3">
            <div class="listItem">
              <div class="inner">
                <a href="#" ><div class="thumb"/></a>
              </div>
            </div>
          </div>
          <div class="list col-sm-3">
            <div class="listItem">
              <div class="inner">
                <a href="#" ><div class="thumb"/></a>
              </div>
            </div>
          </div>
          <div class="list col-sm-3">
            <div class="listItem">
              <div class="inner">
                <a href="#" ><div class="thumb"/></a>
              </div>
            </div>
          </div>
          <div class="list col-sm-3">
            <div class="listItem">
              <div class="inner">
                <a href="#" ><div class="thumb"/></a>
              </div>
            </div>
          </div>
          <div class="list col-sm-3">
            <div class="listItem">
              <div class="inner">
                <a href="#" ><div class="thumb"/></a>
              </div>
            </div>
          </div>
          <div class="list col-sm-3">
            <div class="listItem">
              <div class="inner">
                <a href="#" ><div class="thumb"/></a>
              </div>
            </div>
          </div>
          <div class="list col-sm-3">
            <div class="listItem">
              <div class="inner">
                <a href="#" ><div class="thumb"/></a>
              </div>
            </div>
          </div>
          <div class="list col-sm-3">
            <div class="listItem">
              <div class="inner">
                <a href="#" ><div class="thumb"/></a>
              </div>
            </div>
          </div>
          <div class="list col-sm-3">
            <div class="listItem">
              <div class="inner">
                <a href="#" ><div class="thumb"/></a>
              </div>
            </div>
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
  @import "~/assets/scss/library/variable.scss";
  @import "~/assets/scss/library/mixin.scss";

  .p-sponsor {

    background-color:#FAEAE6;
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

      @include desktop {
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
      @include desktop {
        padding: 50px 0 0;
      }

      .inner {
        width: 100%;
        margin: 0 auto 30px;
        padding: 0 30px;
        display: inline-block;
        text-align: left;
        box-sizing: border-box;

        @include desktop {
          margin: 0 auto 40px;
        }
      }
    }

    &_platinum {
      margin-bottom: 30px;
      @include desktop {
        margin-bottom: 60px;
      }

      @include desktop {

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

          @include desktop {
            max-width: 600px;
          }
        }

      }
    }

    &_gold {
      margin-bottom: 30px;
      @include desktop {
        margin-bottom: 60px;
      }
      .list {

      }
      .listItem {
        .inner {
          max-width: 100%;
          @include desktop {
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

          @include desktop {
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
      @include desktop {
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

        @include desktop {
          margin-bottom: 30px;
        }

        .inner {
          margin-bottom: 20px;
          width: 100%;
          padding: 0 20px;
          @include desktop {
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

          @include desktop {
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
      @include desktop {
        margin-bottom: 60px;
      }

      .list {
        box-sizing: border-box;
        width: calc( 100% / 3 );
        padding-right: 5px;
        padding-left: 5px;

        @include desktop {
          padding-right: 15px;
          padding-left: 15px;
        }

      }

      .listItem {
        margin-bottom: 10px;
        padding-top: 10px;
        @include desktop {
          margin-bottom: 30px;
          padding-top: 20px;
        }
        .inner {
          margin-bottom: 5px;
          max-width: 220px;
          text-align: center;
          padding: 0 10px;
          @include desktop {
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
