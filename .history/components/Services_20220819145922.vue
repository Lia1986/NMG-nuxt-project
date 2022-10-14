<template>
  <div class="wr_services app_padding">
    <h1 class="title_section">Services</h1>
    <div class="wr_content"></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      srevicesData: [
        { id: 1, title: "Construction", description: "Isalation", icon: "" },
        { id: 2, title: "Sanitary", description: "Isalation", icon: "" },
        { id: 3, title: "Renovation", description: "Isalation", icon: "" },
        { id: 4, title: "Building", description: "Isalation", icon: "" },
        { id: 5, title: "Isalation", description: "Isalation", icon: "" },
        { id: 6, title: "Construction", description: "Isalation", icon: "" },
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