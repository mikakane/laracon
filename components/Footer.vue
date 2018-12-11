<template>
  <div class="l-footer">
    <div class="box">
      <div class="copywriter">
        <p>© 2019 Laravel JP Conference 実行委員会</p>
      </div>
    </div>
  </div>
</template>

<script>
</script>

<style lang="scss" scoped>
  @import "~/assets/scss/library/variable.scss";
  @import "~/assets/scss/library/mixin.scss";

  .box {
    background-color: $clr_footerBackground;
  }

  .copywriter {
    color:#FFF;
    text-align: center;
    padding: 37px 0px 33px;
    font-size:18px;
  }
</style>
