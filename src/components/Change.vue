<template>
  <div>
    <el-carousel height="500px">
      <el-carousel-item v-for="item in pics" :key="item.url">
        <img :src="item.url"/>
      </el-carousel-item>
    </el-carousel>
  </div>
</template>

<script>
export default {
  name: "Change",
  data() {
    return {
      pics: [
        { url: require("../assets/logo.png") },
        { url: require("../assets/logo.png") },
      ]
    };
  }
}
</script>

<style scoped>
.el-carousel__item img {
  height: 500px;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n+1) {
  background-color: #d3dce6;
}
</style>