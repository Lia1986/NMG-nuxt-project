<template>
  <div>
    <div class="wr_portfolio">
      <h1 class="title_section">Portfolio</h1>
      <div class="portfolio d-flex">
        <div class="left_part">
          <div class="for_width">
            <h4>Recent projects we completed</h4>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed
              egestas auctor amet pharetra in. A mauris nec pellentesque non sed
              elit
            </p>
            <button class="btn btn_empty">Contact Us</button>
            <div class="arrowes d-flex">
              <div class="arrow_left">
                <svg
                  width="60"
                  height="60"
                  viewBox="0 0 60 60"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <g opacity="0.7">
                    <path
                      d="M28.7808 16.9782C29.2897 16.4689 30.1153 16.4689 30.625 16.9782C31.1343 17.4871 31.1343 18.3131 30.625 18.8224L20.7478 28.6996H46.9913C47.7136 28.6996 48.2996 29.2855 48.2996 30.0079C48.2996 30.7307 47.7136 31.3162 46.9913 31.3162H20.7609L30.6381 41.1934C30.8832 41.4376 31.0208 41.7699 31.0208 42.1157C31.0208 42.462 30.8832 42.7934 30.6381 43.038C30.3931 43.2851 30.0575 43.422 29.7092 43.4175C29.3622 43.4158 29.0291 43.2798 28.7808 43.038L16.6795 30.9372C16.4333 30.6905 16.296 30.3558 16.2997 30.0079C16.3021 29.6609 16.4382 29.329 16.6795 29.0794L28.7808 16.9782Z"
                      fill="white"
                    />
                    <path
                      d="M29.984 1.88094C41.3604 1.87889 51.6175 8.73138 55.971 19.242C60.3236 29.7531 57.916 41.8511 49.8691 49.893C38.8864 60.8757 21.0808 60.8757 10.0985 49.893C-0.883751 38.9112 -0.883751 21.1055 10.0985 10.1229C15.3608 4.83066 22.521 1.86291 29.984 1.88094ZM29.984 55.5188C44.0475 55.5188 55.4944 44.0715 55.4944 30.008C55.4944 15.9444 44.0475 4.49754 29.984 4.49754C15.9205 4.49754 4.47319 15.9444 4.47319 30.008C4.47319 44.0715 15.9205 55.5188 29.984 55.5188Z"
                      fill="white"
                    />
                  </g>
                </svg>
              </div>
              <div>
                <svg
                  width="60"
                  height="60"
                  viewBox="0 0 60 60"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M31.2192 16.9782C30.7103 16.4689 29.8847 16.4689 29.375 16.9782C28.8657 17.4871 28.8657 18.3131 29.375 18.8224L39.2522 28.6996H13.0087C12.2864 28.6996 11.7004 29.2855 11.7004 30.0079C11.7004 30.7307 12.2864 31.3162 13.0087 31.3162H39.2391L29.3619 41.1934C29.1168 41.4376 28.9792 41.7699 28.9792 42.1157C28.9792 42.462 29.1168 42.7934 29.3619 43.038C29.6069 43.2851 29.9425 43.422 30.2908 43.4175C30.6378 43.4158 30.9709 43.2798 31.2192 43.038L43.3205 30.9372C43.5667 30.6905 43.704 30.3558 43.7003 30.0079C43.6979 29.6609 43.5618 29.329 43.3205 29.0794L31.2192 16.9782Z"
                    fill="white"
                  />
                  <path
                    d="M30.016 1.88094C18.6396 1.87889 8.38253 8.73138 4.02904 19.242C-0.323627 29.7531 2.08401 41.8511 10.1309 49.893C21.1136 60.8757 38.9192 60.8757 49.9015 49.893C60.8838 38.9112 60.8838 21.1055 49.9015 10.1229C44.6392 4.83066 37.479 1.86291 30.016 1.88094ZM30.016 55.5188C15.9525 55.5188 4.50557 44.0715 4.50557 30.008C4.50557 15.9444 15.9525 4.49754 30.016 4.49754C44.0795 4.49754 55.5268 15.9444 55.5268 30.008C55.5268 44.0715 44.0795 55.5188 30.016 55.5188Z"
                    fill="white"
                  />
                </svg>
              </div>
            </div>
          </div>
        </div>
        <div class="right_part">
          <div class="itemPort" v-for="item in bildingData" :key="item.id">
            <img :src="require(`@/assets/images/${item.img}`)" alt="img" />
            <span>{{ item.name }}</span>
          </div>
        </div>
      </div>
    </div>
    <div></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      bildingData: [
        { id: 1, img: "portfolio_1.png", name: "Lorem Ipsum" },
        { id: 2, img: "portfolio_2.png", name: "Lorem Ipsum" },
        { id: 3, img: "portfolio_3.png", name: "Lorem Ipsum" },
        { id: 4, img: "portfolio_4.png", name: "Lorem Ipsum" },
        { id: 5, img: "portfolio_5.png", name: "Lorem Ipsum" },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.wr_portfolio {
  padding: 130px 0 219px 0;
  background-image: url("./../assets/images/bg_portfolio.png");
  background-repeat: no-repeat;
  .portfolio {
    .left_part {
      width: 625px;
      height: 728px;
      background-color: $blueMain;
      background-image: url("./../assets/images/workers_portfolio.png");
      background-repeat: no-repeat;
      background-position-y: bottom;
      border-radius: $bRadius;
      padding-top: 80px;
      .for_width {
        width: 426px;
        margin: 0 auto;
      }
      h4 {
        font-family: $font600;
        font-weight: 600;
        font-size: 36px;
        line-height: 44px;
        color: $yellowMain;
      }
      p {
        margin: 36px auto;
        color: $white;
        font-family: $font600;
        font-weight: 500;
        font-size: 18px;
        line-height: 26px;
      }
      .arrowes {
        margin-top: 36px;
        .arrow_left {
          margin-right: 44px;
        }
      }
    }
    .right_part {
      display: flex;
      flex-wrap: wrap;
      .itemPort {
        position: relative;
        margin: 10px;
        span {
          d
          position: absolute;
        }
      }
    }
  }
}
</style>