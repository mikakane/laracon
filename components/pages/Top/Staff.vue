<template>
  <div class="p-staff">
    <div class="parent">
      <img src="~assets/images/staff/staff_left.png" class="c-left">
      <img src="~assets/images/staff/staff_right.png" class="c-right">
    </div>
    <div class="c-container">
      <div class="parent">
        <img src="~assets/images/staff/staff_title.png" class="c-stafftitle">
      </div>

      <div class="title">
        STAFF
      </div>

<div class="box">


      <div class="item">

        <div class="grid">

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>

          <div class="staff">
            <div class="staff-box">
              <div class="img"></div>
              <p class="c-name">
                田中 太郎
              </p>
            </div>
          </div>


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

  .title {
    color: #64547B;
    font-size:4rem;
    font-family: playfair-display; //ここが適用されない
    font-weight: bold;
    text-align:left;
    margin-bottom:3.4rem;
    position: relative
  }

  .staff-box{
    max-width:150px;
    text-align:center;
  }


  .img{
    width:70px;
    height:70px;
    background-color: #eee;
    border-radius:50%;
    display:inline-block;
  }

  .c-name{
    color: #64547B;
    font-size: 1.6rem;
    display: inline-block;
    text-align:center;
  }

  .grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    justify-items: center;
    @include desktop {
      grid-template-columns: repeat(6, 1fr);

    }
  }

  .item{
    grid-area: item;
    display: flex;
    justify-content:  start;

  }
  .box{
    display: flex;
    position: relative;
    z-index:999;
  }

  .c-stafftitle {
    position: absolute;
    max-height: 390px;
    top: -70px;
    right:0px;
    opacity: 0;
    @include desktop{
      position: absolute;
      max-height: 390px;
      top: -70px;
      right:0px;
      opacity: 100;
    }

  }

  .c-left {
    position: absolute;
    max-width: 390px;
    top: 100px;
    left:0px;
    max-width: 100%;
    z-index:99;
  }

  .c-right {
    position: absolute;
    max-width: 470px;
    top: 100px;
    right:0px;
    z-index:99;
  }

  .parent{
    position: relative;
    z-index:99;
  }
</style>

