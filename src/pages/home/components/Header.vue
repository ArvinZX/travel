<template>
    <div class="header">
      <div class="header-left">
        <div class="iconfont icon-back">&#xe624;</div>
      </div>
      <div class="header-input">
        <span class="iconfont">&#xe632;</span>
        输入城市/景点/游玩主题
      </div>
      <div class="header-right">
        城市
        <span class="iconfont icon-arrow">&#xe64a; </span>
      </div>
    </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>
  @import "~styles/varibles.styl"
  .header
    display flex
    line-height :.86rem
    background: $bgcolor
    color: #fff
    .header-left
      width: .64rem
      float: left
      .icon-back
        text-align :center
        font-size : .4rem
    .header-input
      flex:1
      height .62rem
      line-height : .62rem
      margin-top :.12rem
      margin-left :.2rem
      background :#fff
      border-radius :.1rem
      color :#ccc
      padding-left : .2rem
    .header-right
      width:1.24rem
      float: right
      text-align:center
      .icon-arrow
        margin-left : -.04rem
        font-size: 0.24rem
</style>
