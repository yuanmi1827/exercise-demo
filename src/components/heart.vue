<template>
  <div id="wraper">
    <div id="heart">
      <svg t="1587910011145" class="item" viewBox="0 0 1024 1024" version="1.1" p-id="1253" width="32" height="32">
        <path d="M677.51936 192.03072c113.1008 0 204.8 91.6992 204.8 204.77952 0
          186.91072-370.3296 435.15904-370.3296 435.15904S141.68064 592.67072 141.68064
          396.81024c0-140.78976 91.6992-204.77952 204.77952-204.77952 68.11648 0
          128.28672 33.40288 165.5296 84.55168C549.24288 225.4336 609.41312 192.03072
          677.51936 192.03072z" p-id="1254"
        ></path>
      </svg>
    </div>
  </div>
</template>


<script type='text/ecmascript-6'>
  export default {
    name: 'heart',
    data () {
      return {
      }
    },
    created() {
    },
    mounted() {
      this.createdHearts()
      this.setAnimate()
    },
    methods: {
      //循环生成多个爱心
      createdHearts() {
        let heartList = ''
        const n = 99
        for (let i = 0; i < n; i++) {
          heartList += `<svg id="heart_${i} class="ani" t="1587910011145" viewBox="0 0 1024 1024" version="1.1" p-id="1253" width="32" height="32">
            <path d="M677.51936 192.03072c113.1008 0 204.8 91.6992 204.8 204.77952 0
              186.91072-370.3296 435.15904-370.3296 435.15904S141.68064 592.67072 141.68064
              396.81024c0-140.78976 91.6992-204.77952 204.77952-204.77952 68.11648 0
              128.28672 33.40288 165.5296 84.55168C549.24288 225.4336 609.41312 192.03072
              677.51936 192.03072z" p-id="1254"
              fill=${this.getRandomColor()}
            ></path>
          </svg>`
        }
        document.getElementById('heart').innerHTML = heartList
      },
      //生成随机色
      getRandomColor() {
        const r= Math.floor(Math.random()*255)
        const g = Math.floor(Math.random()*255)
        const b = Math.floor(Math.random()*255)
        return 'rgba('+ r +','+ g +','+ b +',0.8)'
      },
      //set animate
      setAnimate() {
        const n = 99
        const boxWidth = window.innerWidth
        const boxHeight = window.innerHeight
        setTimeout(() => {
          for (let i = 0; i < n; i++) {
            const width = this.getRandomNum(boxWidth)
            const height = this.getRandomNum(boxHeight)
            const cWidth = this.getRandomNum(1000) - width
            const cHeight = this.getRandomNum(1000) - height
            document.getElementsByTagName('svg')[i].animate([
              {transform: `scale(${this.getRandomNum(2)})`,left: `0px`, top: `0px` },
              {transform: `scale(${this.getRandomNum(2)})`,left: `${boxWidth/2}px`, top: `${boxHeight/2}px` },
              {transform: `scale(${this.getRandomNum(2)})`,left: `${cWidth * 2}px`, top: `${cHeight * 2}px` },
            ], {
              duration: 9000,
              iterations: Infinity,
              easing: 'ease-in-out'
            })
          }
        }, 100)
      },
      //动画随机数
      getRandomNum(scale) {
        return Math.floor(Math.random()*scale+1)
      }

    }
  }
</script>

<style lang='stylus' rel='stylesheet/stylus' scoped>
  #wraper
    width 100%
    height 100%
    overflow hidden
    #heart
      position 
      .ani
        position absolute
</style>