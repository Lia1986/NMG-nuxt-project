<template>
  <div>
    <WorkingProcess />
    <AboutUs/>
    <Services/>
    <Portfolio
  </div>
</template>

<script>
import WorkingProcess from "./WorkingProcess.vue";
import AboutUs from "./AboutUs.vue";
import Services from "./Services.vue";
export default {
  name: "Home",
  component: {
    WorkingProcess,
    AboutUs,
    Services,
  },
};
</script>
