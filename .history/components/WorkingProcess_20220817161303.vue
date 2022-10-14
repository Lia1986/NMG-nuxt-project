<template>
  <div class="wr_working_proccess app_padding">
    <h1>Our working proccess</h1>
    <div class="wr_content">
      <div
        class="content_item d-flex_jc-c_ai-c jc_sb"
        v-for="(item, index) in workingProccess"
        :key="item.id"
      >
        <div class="d-flex_jc-c_ai-c">
          <div style="position: relative">
            <div
              v-if="workingProccess.length - 1 != index"
              class="dashed_border"
            ></div>
            <div
              v-if="workingProccess.length - 1 === index"
              class="end_proccess_dashed"
            ></div>
            <div class="proccess_step mr-20">0{{ item.id }}</div>
          </div>
          <div class="item_info">
            <h3 class="mb-12">{{ item.title }}</h3>
            <p>{{ item.description }}</p>
          </div>
        </div>
        <div><img :src="require(`@/assets/images/${item.img}`)" alt="" /></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      workingProccess: [
        {
          id: 1,
          title: "Acceptance of order and discussion",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          img: "img_working_proccess-1.png",
        },
        {
          id: 2,
          title: "Visit to the construction site",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          img: "img_working_proccess-2.png",
        },
        {
          id: 3,
          title: "Discussion of date and price",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque.",
          img: "img_working_proccess-3.png",
        },
        {
          id: 4,
          title: "Start of work",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          img: "img_working_proccess-4.png",
        },
        {
          id: 5,
          title: "Ongoing discussions",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          img: "img_working_proccess-5.png",
        },
        {
          id: 6,
          title: "Job transfer",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          img: "img_working_proccess-6.png",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.wr_working_proccess {
  padding-top: 130px;
  h1 {
    color: $yellowMain;
    text-align: center;
    font-weight: 600;
    font-size: 36px;
    margin-bottom: 80px;
  }
  .content_item {
    margin-bottom: 80px;
    .item_info {
      width: 569px;
      color: $blueMain;
      h3 {
        font-weight: 600;
        font-size: 24px;
        line-height: 32px;
      }
      p {
        font-weight: 500;
        font-size: 18px;
        line-height: 26px;
      }
    }
    .proccess_step {
      font-weight: 900;
      font-size: 96px;
      opacity: 0.4;
      color: $yellowMain;
    }
    .dashed_border {
      position: absolute;
      left: -65px;
      top: 55px;
      width: 62px;
      height: 438px;
      border-top: 2px dashed $yellowMain;
      border-left: 2px dashed $yellowMain;
    }
    .end_proccess_dashed {
      position: absolute;
      left: -65px;
      top: 55px;
      width: 62px;
      border-top: 2px dashed $yellowMain;
    }
  }
}
</style>