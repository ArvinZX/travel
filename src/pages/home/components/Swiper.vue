<template>
  <div class="swiper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide  v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl">
      </swiper-slide>
<!--      <swiper-slide>-->
<!--        <img class="swiper-img" src="http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20199/4c232af79d5ee2826994519d5ced0ed0.jpg_750x200_5ec9be08.jpg" alt="">-->
<!--      </swiper-slide>-->
      <!--    <swiper-slide>I'm Slide 3</swiper-slide>-->
      <!--    <swiper-slide>I'm Slide 4</swiper-slide>-->
      <!--    <swiper-slide>I'm Slide 5</swiper-slide>-->
      <!--    <swiper-slide>I'm Slide 6</swiper-slide>-->
      <!--    <swiper-slide>I'm Slide 7</swiper-slide>-->
      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
      <!--    <div class="swiper-button-prev" slot="button-prev"></div>-->
      <!--    <div class="swiper-button-next" slot="button-next"></div>-->
      <!--    <div class="swiper-scrollbar"   slot="scrollbar"></div>-->
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperList: [
        {
          id: '0001',
          imgUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20199/5adf9fd5c515026fd5e9ef6fc89dad5e.jpg_750x200_6f045c57.jpg'
        }, {
          id: '0002',
          imgUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20199/4c232af79d5ee2826994519d5ced0ed0.jpg_750x200_5ec9be08.jpg'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .swiper >>> .swiper-pagination-bullet-active
    background : #fff
  .swiper
    overflow: hidden
    width : 100%
    height : 0
    padding-bottom : 31.25%
    .swiper-img
      width : 100%
</style>
