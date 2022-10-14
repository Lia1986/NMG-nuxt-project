<template>
  <div class="wr_about_us app_padding">
    <h1 class="title_section">About Us</h1>
    <div class="wr_content d-flex_jc-c_ai-c ai_fs">
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
        <div class="wr_indicator d-flex_jc-c_ai-c jc_sb">
          <div
            class="item_indicator"
            v-for="item in indicatorData"
            :key="item.id"
          >
            <div class="d-flex">
              <img
                :src="require(`@/assets/images/svg/${item.icon}`)"
                alt="icon"
              />
              {{ item.quantity }}
            </div>
            <h6>{{ item.title }}</h6>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      indicatorData: [
        { id: 1, title: "happy clients", icon: "happy.svg", quantity: "130+" },
        {
          id: 2,
          title: "years of experience",
          icon: "years.svg",
          quantity: "10+",
        },
        {
          id: 3,
          title: "Finished projects",
          icon: "finished_projects.svg",
          quantity: "220+",
        },
        { id: 4, title: "happy clients", icon: "happy.svg", quantity: "130+" },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.wr_about_us {
  margin-bottom: 174px;
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
      position: relative;
      p {
        font-family: $font500;
        font-weight: 500;
        font-size: 18px;
        line-height: 26px;
      }
      .wr_indicator {
        position: absolute;
        width: 1000px;
        padding: 46px;
        background: $blueMain;
        bottom: -266px;
        left: -467px;
        .item_indicator {
          color: $white;
          h6 {
            margin-top: 8px;
            font-family: $font500;
            font-size: 18px;
          }
          div {
            font-family: $font600;
            font-style: normal;
            font-weight: 600;
            font-size: 36px;
            img {
              margin-right: 12px;
            }
          }
        }
      }
    }
  }
}
</style>