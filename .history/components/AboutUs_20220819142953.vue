<template>
  <div class="wr_about_us app_padding">
    <h1 class="title_section">About Us</h1>
    <div class="wr_content d-flex_jc-c_ai-c ai_fs jc_sb">
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
              <div>
              <img
                :src="require(`@/assets/images/svg/${item.icon}`)"
                alt="icon"
              />
              </div>
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
    width: 100%;
    .left_part {
      div {
        position: relative;
        background: $blueMain;
        width: 34.7vw;
        height: 32.1vw;
        img {
          width: 100%;
          position: absolute;
          top: 2.3vw;
          left: 2.3vw;
        }
      }
    }
    .right_part {
      position: relative;
      p {
        font-family: $font500;
        font-weight: 500;
        font-size: 0.94vw;
        line-height: 1.34vw;
        width: 28.6vw;
      }
      .wr_indicator {
        position: absolute;
        width: 47.3vw;
        padding: 2.4vw;
        background: $blueMain;
        bottom: -15.8vw;
        left: -24.3vw;
        .item_indicator {
          color: $white;
          h6 {
            margin-top: 0.43vw;
            font-family: $font500;
            font-size: 0.94vw;
          }
          div {
            font-family: $font600;
            font-style: normal;
            font-weight: 600;
            font-size: 1.88vw;
            img {
              margin-right: 0.64vw;
            }
          }
        }
      }
    }
  }
}
</style>