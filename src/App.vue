<template>
  <div id="app">
    <header>
      <first-screen />
    </header>
    <main>
      <description />
      <our-history />
      <!-- <our-services /> -->
      <stats />
      <our-pricing />
      <our-clients />
      <our-blog />
      <contacts />
      <free-trial />
    </main>
      <vue-footer />
  </div>
</template>

<script>
import FirstScreen from "./components/FirstScreen.vue";
import Description from "./components/Description.vue";
import OurHistory from "./components/OurHistory.vue";
import OurServices from "./components/OurServices.vue";
import VueFooter from "./components/VueFooter.vue";
import FreeTrial from "./components/FreeTrial";
import Contacts from "./components/Contacts";
import OurBlog from "./components/OurBlog";
import OurClients from "./components/OurClients";
import OurPricing from "./components/OurPricing";
import Stats from "./components/Stats";

export default {
  name: "app",
  components: {
    FirstScreen,
    Description,
    OurHistory,
    OurServices,
    VueFooter,
    FreeTrial,
    Contacts,
    OurBlog,
    OurClients,
    OurPricing,
    Stats,
  },
};
</script>

<style lang="scss"></style>
