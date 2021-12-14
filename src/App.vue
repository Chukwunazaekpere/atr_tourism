<template>
  <Banner />
  <History />
  <!-- <Footer /> -->
</template>

<script lang="ts">
import { defineComponent } from "vue";
// import Footer from "@/components/Footer.vue";
import Banner from "@/components/Banner.vue";
import History from "@/components/History.vue";


export default defineComponent({
  name: "App",
  components: {
    // Footer,
    History,
    Banner,
  },
});
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
