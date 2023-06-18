<template>
  <div class="content">
    <div class="content__col col-left">
      <DesktopBestSelling />
      <div class="col__featured">
        <div class="content__col">
          <ProgresBarDesktop />
          <WaveLineChartDesktop />
        </div>
        <div class="content__col">
          <WaveChart />
          <PieChartDesktop />
        </div>
      </div>
    </div>
    <div class="content__col col-right">
        <BarChart/>
        <SliderImage/>
    </div>
    
  </div>
</template>

<script>
import DesktopBestSelling from "./DesktopBestSelling.vue";
import ProgresBarDesktop from "./ProgresBarDesktop.vue";
import WaveChart from "./WaveChart.vue";
import WaveLineChartDesktop from "./WaveLineChartDesktop.vue";
import PieChartDesktop from "./PieChartDesktop.vue";
import BarChart from "./BarChart.vue";
import SliderImage from "./SliderImage.vue";

export default {
  name: "HomeContentDesktop",
  components: {
    DesktopBestSelling,
    ProgresBarDesktop,
    WaveLineChartDesktop,
    WaveChart,
    PieChartDesktop,
    BarChart,
    SliderImage
  },
};
</script>

<style scoped>
.content {
  display: flex;
  flex-direction: row;
  margin: 3vw 3.23vw;
}
.content__col {
  width: 50%;
}

.col__featured {
  display: flex;
  flex-direction: row;
}

.col-right {
    margin-left: 1vw;
}
.col-left {
    margin-right: 1vw;
}
</style>
