<template>
  <div class="wr_services app_padding">
    <h1 class="title_section">Services</h1>
    <div class="wr_content">
      <div class="item_services" v-for="item in srevicesData" :key="item.id">
        <div class="icon">
          <img :src="require(`@/assets/images/svg/${item.icon}`)" alt="" />
        </div>
        <h3>{{ item.title }}</h3>
        <p>{{ item.description }}</p>
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
          icon: "construction_1.svg",
        },
        {
          id: 2,
          title: "Sanitary",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          icon: "sanitary.svg",
        },
        {
          id: 3,
          title: "Renovation",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          icon: "renovation.svg",
        },
        {
          id: 4,
          title: "Building",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          icon: "building.svg",
        },
        {
          id: 5,
          title: "Isalation",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          icon: "isalation.svg",
        },
        {
          id: 6,
          title: "Construction",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Rhoncus ut ut vehicula massa fringilla pellentesque. ",
          icon: "construction_6.svg",
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
  .item_services{
    bac
  }
}
</style>