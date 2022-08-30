<template>
  <div class="sensor-picker">
    <div class="row">
      <img src="../assets/temperature.svg" alt="Температура" class="temperature-image">
    </div>
    <div class="row content-column">
      <div class="row-column">Температура</div>
      <div class="row-column">24 &deg;C</div>
    </div>
    <div class="row">
      <img src="../assets/select.svg" alt="Температура" class="select-image">
    </div>
  </div>
</template>

<script>
export default {
  name: "SensorPicker"
}
</script>

<style scoped>
.sensor-picker {
  padding: 8px 20px;
  display: flex;
}

.sensor-picker .row {
  display: flex;
  justify-content: center;
  align-items: baseline;
  height: 64px;
  flex-direction: column;
  flex-wrap: nowrap;
  align-content: center;
}

.content-column {
  margin-left: 15px;
  width: 178px;
  font-size: 1.2rem;
}
</style>