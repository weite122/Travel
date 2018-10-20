<template>
  <div class="banner">
    <img class="banner-img" src="//img1.qunarzz.com/sight/p0/1810/14/14b8a787d6e901f6a3.img.jpg_600x330_7ee67553.jpg" alt="">
    <div class="banner-info">
      <div class="banner-title">
        杭州云曼温泉
      </div>
      <div class="banner-number">
        <span class="iconfont banner-icon">&#xe632;</span>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "DetailBanner"
  }
</script>

<style lang="stylus" scoped>
  .banner
    position: relative
    overflow: hidden
    height: 0
    padding-bottom: 55%
    .banner-img
      width: 100%
    .banner-info
      position: absolute
      left: 0
      right: 0
      right: 0
      bottom: 0
      line-height :.6rem
      color: #fff
      .banner-title
        flex: 1
        font-size: .32rem
        padding: 0 .2rem
      .banner-number
        padding: 0 .4rem
        margin-top: .2rem
        height: .32rem
        line-height: .32rem
        border-radius: .2rem
        background: rgba(0, 0, 0, .8)
        font-size: .24rem
        .banner-icon
          font-size: .24rem
</style>
