<template>
  <div class="wr_services app_padding">
    <h1 class="title_section">Services</h1>
    <div class="wr_content">
        <div v-for="item in srevicesData" :key="item.id">
            <div class="icon">
                :<img src="" alt="">
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      srevicesData: [
        {
          id: 1,
          title: "Construction",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          icon: "construction_1",
        },
        {
          id: 2,
          title: "Sanitary",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          icon: "sanitary",
        },
        {
          id: 3,
          title: "Renovation",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          icon: "renovation",
        },
        {
          id: 4,
          title: "Building",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          icon: "building",
        },
        {
          id: 5,
          title: "Isalation",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          icon: "isalation",
        },
        {
          id: 6,
          title: "Construction",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          icon: "construction_6",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.wr_services {
  background: $blueMain;
  padding-top: 60px;
  padding-bottom: 140px;
}
</style>