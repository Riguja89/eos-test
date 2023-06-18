<template>
  <div class="wave-chart">
    <img src="../assets/images/waveChart.png" alt="" />
  </div>
</template>

<style scoped>
.wave-chart img {
  width: 100%;
  height: 100%;
  border-radius: 1vw;
}

.wave-chart {
  margin: 1vw 0 1vw 0.8vw;
}
@media screen and (max-width: 990px) {
.wave-chart img {
  width: 92%;
  border-radius: 4vw;
}
.wave-chart {
  margin-right: 1vw;
  margin-left: 1vw;
  margin-bottom: 4vw;
}
}
</style>
