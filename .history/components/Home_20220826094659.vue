<template>
  <div>
    <WorkingProcess />
    <AboutUs />
    <Services />
    <Portfolio />
    <Partners />
    <ContactUs
  </div>
</template>

<script>
import WorkingProcess from "./WorkingProcess.vue";
import AboutUs from "./AboutUs.vue";
import Services from "./Services.vue";
import Portfolio from "./Portfolio.vue";
import Partners from "./Partners.vue";
import ContactUs from "./ContactUs.vue";
export default {
  name: "Home",
  component: {
    WorkingProcess,
    AboutUs,
    Services,
    Portfolio,
    Partners,
    ContactUs,
  },
};
</script>
