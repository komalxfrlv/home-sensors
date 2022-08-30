<template>
  <div class="home">
    <div class="blue-boxes">
      <div class="sensor-picker-holder">
        <BlueBox class="blue-box">
          <SensorPicker></SensorPicker>
        </BlueBox>
      </div>
      <div class="time-viewer-holder">
        <BlueBox class="blue-box">
          <TimeViewer></TimeViewer>
        </BlueBox>
      </div>
    </div>
    <div class="chart">
      <SensorChart></SensorChart>
    </div>
  </div>
</template>
<script>
import SensorPicker from "@/components/SensorPicker";
import BlueBox from "@/components/BlueBox";
import TimeViewer from "@/components/TimeViewer";
import SensorChart from "@/components/SensorChart";

export default {
  name: 'HomeView',
  components: {
    SensorChart,
    BlueBox,
    SensorPicker,
    TimeViewer,
  }
}
</script>
<style scoped>
.blue-box {
  max-width: 300px;
}
.blue-boxes {
  display: flex;
  justify-content: space-between;
}
.chart {
  margin-top: 100px;
}
</style>