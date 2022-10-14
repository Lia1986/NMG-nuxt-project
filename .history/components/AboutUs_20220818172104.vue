<template>
  <div class="wr_about_us app_padding">
    <h1 class="title_section">About Us</h1>
    <div class="wr_content d-flex_jc-c_ai-c">
      <div class="left_part">
        <div>
          <img src="@/assets/images/img_about.png" alt="" />
        </div>
      </div>
      <div class="right_part">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed egestas
          auctor amet pharetra in. A mauris nec pellentesque non sed elit. Diam,
          arcu, urna, integer amet convallis cras arcu.Lorem ipsum dolor sit
          amet, consectetur adipiscing elit. Sed egestas auctor amet pharetra
          in. A mauris nec pellentesque non sed elit. Diam, arcu, urna, integer
          amet convallis cras arcu. Lorem ipsum dolor sit amet, consectetur
          adipiscing elit. Sed egestas auctor amet pharetra in. A mauris nec
          pellentesque non sed elit. Diam, arcu, urna, integer amet convallis
          cras arcu.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed
          egestas auctor amet pharetra in. A mauris nec pellentesque non sed
          elit. Diam, arcu, urna, integer amet convallis cras arcu.
        </p>
        <div class="wr_indicator"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.wr_about_us {
  .wr_content {
    .left_part {
        margin-right: 140px;
      div {
        position: relative;
        background: $blueMain;
        width: 666px;
        height: 616px;
        img {
          position: absolute;
          top: 44px;
          left: 44px;
        }
      }
    }
    .right_part {
      p {
        font-family: $font500;
        font-weight: 500;
        font-size: 18px;
        line-height: 26px;
      }
      .wr_indicator{
        padding: 46px;
        background: ;
      }
    }
  }
}
</style>