<template>
  <div class="about">
    <span class="num">213</span>
    <el-input v-model="input" placeholder="Please input" />
    <el-button type="success" @click="getInput()">getInput</el-button>
  </div>
  <div class="about2">
    <span class="num">123</span>
  </div>
</template>

<script>
export default {
  data() {
    return {
      input: "",
    };
  },
  methods: {
    getInput: function () {
      console.log(this.input);
    },
  },
};
</script>

<style lang="less" scoped>
@import "@/assets/index.less";
.num {
  color: @color-blue;
}
.about {
  width: 100%;
  min-height: 100vh;
  display: flex;
  align-items: center;
  .num {
    color: @color-red;
  }
}
.about2 {
  width: 100px;
  height: 50px;
  border: @border;
  .test();
}
/deep/ .el-input {
  .el-input__wrapper {
    background: @text-red;
    .el-input__inner {
      background: @text-red;
    }
  }
}
</style>
