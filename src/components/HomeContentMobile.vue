<template>
    <BestSelling />
    <PcsSoldCounter />
    <WaveChart />
    <PieChart />
    <SliderImage />
  </template>
  
  <script>
 import BestSelling from "./BestSelling.vue";
import PcsSoldCounter from "./PcsSoldCounter.vue";
import WaveChart from "./WaveChart.vue";
import PieChart from "./PieChart.vue";
import SliderImage from "./SliderImage.vue";
  
  export default {
    name: "HomeContentDesktop",
    components: {
    BestSelling,
    PcsSoldCounter,
    WaveChart,
    PieChart,
    SliderImage,
    },
  };
  </script>
  
  <style scoped>
  
  </style>