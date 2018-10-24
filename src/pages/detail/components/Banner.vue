<template>
  <div>
    <div class="banner" @click="handleBannerClick">
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
    <common-gallery
      :imgs="imgs"
      v-show="showGallery"
      @close="handleGalleryClose"
    ></common-gallery>
  </div>
</template>

<script>
  import CommonGallery from 'common/gallery/Gallery'
  export default {
    name: "DetailBanner",
    data() {
      return {
        showGallery: false,
        imgs: ['http://img1.qunarzz.com/sight/p0/1810/cc/cc47164357acbeb5a3.water.jpg_350x240_e25fa3ed.jpg',
          'http://img1.qunarzz.com/sight/p0/1810/eb/ebc93493af1a3189a3.water.jpg_350x240_31e50f11.jpg']
      }
    },
    methods: {
      handleBannerClick () {
        this.showGallery =  true
      },
      handleGalleryClose () {
        this.showGallery =  false
      }
    },
    components: {
      CommonGallery
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
