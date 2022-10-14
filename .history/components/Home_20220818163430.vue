<template>
  <div>
    <WorkingProcess />
    <AboutUs
  </div>
</template>

<script>
import WorkingProcess from "./WorkingProcess.vue";
import AboutUs from "./AboutUs.vue";
export default {
  name: "Home",
  component: {
    WorkingProcess,
    AboutUs,
  },
};
</script>
