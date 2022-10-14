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
        { id: 1, title: "", description: "", icon: "" },
        { id: 2, title: "", description: "", icon: "" },
        { id: 3, title: "", description: "", icon: "" },
        { id: 4, title: "", description: "", icon: "" },
        { id: 5, title: "", description: "", icon: "" },
        { id: 6, title: "", description: "", icon: "" },
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