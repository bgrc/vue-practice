<template>
  <div class="icons">
    <swiper :options="swiperOption">
      <swiper-slide>
        <div v-for="(item, index) in iconList1" :key="index">
          <div class="icon-item">
            <img :src='item.imgUrl' />
            <p class="keywords">{{item.keywords}}</p>
          </div>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div v-for="(item, index) in iconList2" :key="index">
          <div class="icon-item">
            <img :src='item.imgUrl' />
            <p class="keywords">{{item.keywords}}</p>
          </div>
        </div>
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeIcons',
  data () {
    return {
      swiperOption: {
        pagination: {
          el: '.swiper-pagination'
        }
      },
      iconList1: [
        {
          id: '001',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
          keywords: '景点门票'
        },
        {
          id: '002',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/20/831d62d2e1c7be02.png',
          keywords: '文化古迹'
        },
        {
          id: '003',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/e3/67df61427c8e1302.png',
          keywords: '演出'
        },
        {
          id: '004',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png',
          keywords: '一日游'
        },
        {
          id: '005',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png',
          keywords: '西安必游'
        },
        {
          id: '006',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/76/eb88861d78fb9902.png',
          keywords: '动植物园'
        },
        {
          id: '007',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/ab/6f7d6e44963c9302.png',
          keywords: '泡温泉'
        },
        {
          id: '008',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/fa/2548667cb6e902.png',
          keywords: '逛博物馆'
        }
      ],
      iconList2: [
        {
          id: '009',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/50/26ffa31b56646402.png',
          keywords: '亲子游'
        },
        {
          id: '010',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/80/416c6ab3368d1f02.png',
          keywords: '全部玩乐'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/varibles.styl'
.icons
  height 3.7rem
  overflow hidden
  .swiper-container
    height 100%
  >>>.swiper-pagination-bullet-active
    background rgba(0, 175, 190, 0.8)
  >>>.swiper-pagination-bullet
    width 6px
    height 6px
  .icon-item
    width 25%
    heigh 1.5rem
    float left
    padding-top 0.1rem
    text-align center
    img
      display inline-block
      width 1.1rem
      height 1.1rem
    .keywords
      color $darkTextColor
      font-size 0.28rem
      margin-top 0.1rem
</style>
