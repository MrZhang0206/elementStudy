<template>
  <div class="leftAv"><img :src="sword" /></div>
</template>
<script>
export default {
  name: "SwordLeft",
  data() {
    return {
        sword: new URL('/src/assets/jianling.png', import.meta.url)
    };
  },
};
</script>
<style lang="less" scoped>
@import "@/assets/swordLeft.less";
</style>
