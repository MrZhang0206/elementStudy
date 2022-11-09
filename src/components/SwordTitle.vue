<template>
  <div class="title">
    <div class="navigate">
      <span class="content">首页</span>
      <span>周边商城</span>
      <div class="split">|</div>
    </div>
    <div class="navigate">
      <span class="content">游戏资料</span>
      <span>游戏特色</span>
      <span>职业介绍</span>
      <span>新手指南</span>
      <span>攻略中心</span>
      <div class="split">|</div>
    </div>
    <div class="navigate">
      <span class="content">下载中心</span>
      <span>下载客户端</span>
      <span>南天国体验服</span>
      <span>特色新区</span>
      <div class="split">|</div>
    </div>
    <div class="navigate">
      <span class="content">自助服务</span>
      <span>安全模式</span>
      <span>处罚减免</span>
      <span>封停查询</span>
      <span>工作室清除</span>
      <span>个人中心</span>
      <span>剑灵知己</span>
      <div class="split">|</div>
    </div>
    <div class="navigate">
      <span class="content">玩家互动</span>
      <span>灵芝圈社区</span>
      <span>剑灵微博</span>
      <span>官方论坛</span>
      <div class="split">|</div>
    </div>
    <div class="navigate">
      <span class="content">腾讯客服</span>
      <span>客服专区</span>
      <span>用户协议</span>
      <span>玩家条例</span>
      <span>联系客服</span>
    </div>
  </div>
</template>
<script>
export default {
  name: "SwordTitle",
  data() {},
};
</script>
<style lang="less" scoped>
@import "@/assets/swordTitle.less";
.title {
  display: flex;
  transition: height 0.7s;
  height: @height;
  padding-top: 35px;
  .navigate {
    width: @width;
    height: 100%;
    .display();
    position: relative;
    overflow: hidden;
    color: red;
    line-height: 30px;
    .content {
      font-size: 16px;
    }
    .split {
      position: absolute;
      left: 140px;
      top: 0;
    }
    span {
      font-size: @font-size;
      cursor: pointer;
    }
    span:hover {
      .hoverColor();
    }
  }
}
.title:hover {
  height: 270px;
  background-image: linear-gradient(rgba(0, 0, 0, 1), rgba(255, 255, 255, 0));
}
</style>
