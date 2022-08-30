<template>
  <div class="blue-box">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: "BlueBox"
}
</script>

<style scoped>
.blue-box {
  background: #3D99EF;
  padding: 5px;
  color: white;
  border-radius: 15px;
}
</style>