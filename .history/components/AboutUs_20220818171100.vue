<template>
  <div class="wr_about_us">
    <h1 class="title_section">About Us</h1>
    <div class="wr_content d-flex_jc-c_ai-c">
        <div class="left_part">
            <div>
                <img src="@/assets/images/img_about.png" alt="">
            </div>
        </div>
        <div class="right_part"></div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.wr_about_us{
    .wr_content{
        .left_part{
            div{
                position: relative;
               background: $blueMain; 
               width: 666px;
               
               img{
                position: absolute;
                top: 44px;
               }
            }
        }
    }
}
</style>