<template>
  <div class="content">
    <NavigationDesktop v-if="!mobileView" />
    <NavigationMobile v-if="mobileView" />
    <HomeContentDesktopVue v-if="!mobileView" />
    <HomeContentMobile v-if="mobileView" />
  </div>
</template>

<script>
import NavigationDesktop from "./components/NavigationDesktop.vue";
import NavigationMobile from "./components/NavigationMobile.vue";
import HomeContentDesktopVue from "./components/HomeContentDesktop.vue";
import HomeContentMobile from "./components/HomeContentMobile.vue";

export default {
  name: "App",
  components: {
    NavigationMobile,
    NavigationDesktop,
    HomeContentDesktopVue,
    HomeContentMobile,
  },
  data() {
    return {
      show: false,
      mobileView: false,
      showNav: false,
    };
  },
  methods: {
    handleView() {
      this.mobileView = window.innerWidth <= 990;
    },
  },
  created() {
    this.handleView();
    window.addEventListener("resize", this.handleView);
  },
};
</script>

<style>
@font-face {
  font-family: "Poppins";
  src: url("./assets/fonts/Poppins-Regular.ttf") format("truetype");
}
body {
  margin: 0;
  background-color: #24292e;
}
#app {
  font-family: Poppins, Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
  background-color: #24292e;
  padding-bottom: 12.7vw;
}
@media screen and (min-width: 990px) {
  #app {
    padding-bottom: 0.1vw;
  }
}
</style>
