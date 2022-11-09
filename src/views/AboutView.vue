<template>
  <div class="wholePage">
    <div class="topTitle">
      <SwordTitle />
    </div>
    <div class="swordLeft">
      <SwordLeft />
    </div>
  </div>
</template>

<script>
import SwordTitle from "@/components/SwordTitle.vue";
import SwordLeft from "@/components/SwordLeft.vue";
export default {
  data() {
    return {};
  },
  methods: {},
  components: {
    SwordTitle,
    SwordLeft,
  },
};
</script>

<style lang="less" scoped>
.wholePage {
  background: #eeeeee;
  position: relative;
  .topTitle {
    position: absolute;
    top: 0;
    left: 220px;
  }
}
</style>
