<template>
    <div class="header">
        <div class="header-left">返回</div>
        <!-- <input class="header-input" value="输入城市/景点/游玩主题" /> -->
        <div class="header-input">输入城市/景点/游玩主题</div>
        <div class="header-right">城市</div>
    </div>
</template>

<script>
export default {
  name: "HomeHeader"
};
</script>

<style lang="stylus" scoped>
.header
    display: flex
    flex-direction: row
    justify-content: space-between
    height: 0.86rem
    align-items: center
    background: #00bcd4
    .header-left
        width: 0.64rem
    .header-input
        flex: 1
        color: #ccc
        border-radius: 0.1rem
        margin-left: 0.2rem
        background: #fff
        line-height: 0.64rem
    .header-right
        text-align: center
        width: 1.24rem
</style>
