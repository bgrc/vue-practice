<template>
  <div>
    <h2 class="title">周末去哪</h2>
    <div v-for="(item, index) in weekendList" :key="index">
      <img :src="item.imgUrl">
      <div class="info">
        <p class="name">{{item.name}}</p>
        <p class="desc">{{item.desc}}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
  data () {
    return {
      weekendList: [
        {
          id: '001',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1505/19/58f233e11df7ef.jpg_r_640x214_6b42c9fc.jpg',
          name: '西安必游TOP10',
          desc: '寻长安梦，开启穿越的圆梦之旅'
        },
        {
          id: '002',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1511/14/1cf5dc2ecbfc16.jpg_r_640x214_b4b3a58a.jpg',
          name: '最美丝路行',
          desc: '情系西北，中国梦丝路行'
        },
        {
          id: '003',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1507/fe/679926851c309a.jpg_r_640x214_114816de.jpg',
          name: '不一样的周末',
          desc: '这个周末玩点不一样的'
        },
        {
          id: '004',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1507/98/d9c848b0d7d65a.jpg_r_640x214_55778a01.jpg',
          name: '就是爱大自然',
          desc: '这个周末爬爬山，呼吸呼吸新鲜空气'
        },
        {
          id: '005',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1507/de/e6ba44d61894c0.jpg_r_640x214_847324d0.jpg',
          name: '西安演出在线',
          desc: '没事的时候，西安人最爱在这里观演出'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/mixins.styl'
.title
  height 0.8rem
  padding-left 0.26rem
  line-height 0.8rem
  color #212121
  background #f5f5f5
img
  width 100%
  height 37.4vw
.info
  position relative
  padding 0.14rem 0.2rem 0.2rem 0.2rem
  .name
    color #212121
    font-size 0.28rem
    line-height 0.48rem
    ellipsis()
  .desc
    color #616161
    font-size 0.24rem
    line-height 0.42rem
    ellipsis()
</style>
