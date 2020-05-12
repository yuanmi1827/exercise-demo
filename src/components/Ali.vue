<template>
  <div class="wraper">
    <div class="header" :style="`transform:translateY(${height}px);opacity:${opacity} `">

    </div>
    <div class="scroll" ref="ali">
      <div class="content" ref="content">
        <div class="fill"></div>
        <div class="aaaaa"></div>
      </div>
    </div>
  </div>
</template>

<script type='text/ecmascript-6'>
import BScroll from 'better-scroll'
  export default {
    data () {
      return {
        height:0,
        opacity:1,
        isShow: true
      }
    },
    mounted() {
      setTimeout(() => {
        this._initScroll()
      }, 20)
    },
    methods: {
      _initScroll() {
        const bs = new BScroll(this.$refs.ali, {
          click: true,
          bounce:false,
          probeType:2,
        })
        bs.on('scroll', (pos) => {
          this.height = pos.y*0.8
          if(pos.y<0&&Math.abs(pos.y)>=70) {
            this.isShow = false
          } else {
            this.opacity = this.opacity*0.3
            
          }
          console.log(pos.y,'---------')
          // console.log(this.$refs.content.offsetHeight-document.documentElement.clientHeight)
        })
       
      }
    }
  }
</script>

<style lang='stylus' rel='stylesheet/stylus' scoped>
  .wraper
    width 100%
    height 100%
    position relative
    overflow hidden
    .header
      width 100%
      height 100px
      overflow hidden
      background-color blue
    .scroll
      width 100%
      height 100%
      overflow hidden
      position fixed
      left 0
      top 0
      .content
        position absolute
        top 0
        left 0
        width 100%

        .fill
          width 100%
          height 100px
          background-color transparent
          // background-color pink

        .aaaaa
          width 100%
          height 690px
          background-color red

</style>