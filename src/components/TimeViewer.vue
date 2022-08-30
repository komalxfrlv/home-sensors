<template>
  <div class="time-viewer">
    <div class="row">
      <img src="../assets/time.svg" alt="Время" class="time-image">
    </div>
    <div class="row content-column">
      <div class="row-column">{{ time }}</div>
    </div>
  </div>
</template>

<script>

import moment from 'moment';
export default {
  name: "TimeViewer",
  data() {
    return {
      time: moment().locale('ru').format('LT L')
    }
  },
}
</script>

<style scoped>
.time-viewer {
  padding: 8px 20px;
  display: flex;
}

.time-viewer .row {
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
  font-size: 1.2rem;
}

.time-image {
  height: 64px;
  width: auto;
}
</style>