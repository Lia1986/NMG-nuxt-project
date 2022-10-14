<template>
  <div class="wr_working_proccess">
    <h1></h1>
    <div class="wr_content">
        <div v-for="item in workingProccess" :key></div>
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
</style>