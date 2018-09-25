<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe645;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>
      输入城市/景点/游玩主题
    </div>
    <div class="header-right">
      城市
      <span class="iconfont arrow-icon">&#xe600;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>
@import '~styles/varibles.styl'
.header
  display flex
  flex-direction row
  justify-content space-between
  height 0.86rem
  align-items center
  background $bgcolor
  color #fff
  .header-left
    width 0.77rem
    .back-icon
      text-align center
      font-size 0.36rem
  .header-input
    flex 1
    color #ccc
    border-radius 0.1rem
    background #fff
    line-height 0.6rem
    padding-left 0.2rem
  .header-right
    text-align center
    width 1.24rem
    margin-right 0.1rem
    .arrow-icon
      font-size 0.18rem
      margin-left -0.04rem
</style>
