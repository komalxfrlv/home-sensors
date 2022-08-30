<template>
  <div>
    <line-chart :data="chartData"></line-chart>
  </div>
</template>

<script>
import axios from "axios";

export default {
  name: "SensorChart",
  components: {},
  data() {
    return {
      chartData: null
    }
  },
  mounted() {
    window.setInterval(() => {
      axios
          .get('http://10.11.42.230:1945/ec-fa-bc-51-2f-7c/range/sens1.thermistor.t.c;29.08.2022,19:50:45;30.08.2022,16:55:59')
          .then(response => {
            this.chartData = response.data
          })
    }, 1000)


  }
}
</script>

<style scoped>

</style>
