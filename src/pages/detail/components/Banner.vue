<template>
  <div>
    <div class="banner">
      <img class="banner-img" src="//img1.qunarzz.com/sight/p0/1810/14/14b8a787d6e901f6a3.img.jpg_600x330_7ee67553.jpg" alt="">
      <div class="banner-info">
        <div class="banner-tittle">
          杭州云曼温泉
        </div>
        <div class="banner-number">
          <span class="iconfont banner-icon">&#xe692;</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import CommonGallary from 'common/gallary/Gallary'
  export default {
    name: "DetailBanner",
    components: {
      CommonGallary
    }
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
      display: flex
      position: absolute
      left: 0
      right: 0
      bottom: 0
      line-height: .6rem
      color: #fff
      background-image: linear-gradient(top, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.8))
      .banner-tittle
        flex: 1
        font-size: .32rem
        padding: 0 .2rem
      .banner-number
        height: .32rem
        line-height: .32rem
        margin-top: .14rem
        padding: 0 .4rem
        border-radius: .2remnpm
        background: rgba(0, 0, 0, .8)
        font-size: .24rem
        .banner-icon
          font-size: .24rem
</style>
