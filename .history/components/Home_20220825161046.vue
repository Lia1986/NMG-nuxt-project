<template>
  <div>
    <WorkingProcess />
    <AboutUs />
    <Services />
    <Portfolio />
    <Partners></Partners>
  </div>
</template>

<script>
import WorkingProcess from "./WorkingProcess.vue";
import AboutUs from "./AboutUs.vue";
import Services from "./Services.vue";
import Portfolio from "./Portfolio.vue";
import Partners from "./Partners.vue";
export default {
  name: "Home",
  component: {
    WorkingProcess,
    AboutUs,
    Services,
    Portfolio,
    Partners,
  },
};
</script>
