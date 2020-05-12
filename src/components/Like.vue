<template>
  <div class="wraper">
    <canvas id="thumsCanvas" width="375" height="668"></canvas>
  </div>
</template>

<script type='text/ecmascript-6'>
import ThumbsUpAni from '../common/js/thumbsUpAni'
  export default {
    data () {
      return {
        isshow: false
      }
    },
    mounted() {
      
        let t = new ThumbsUpAni()
      setInterval(()=>{
                t.start();
            },300);
    },
    methods: {
     
    }
  }
</script>

<style lang='stylus' rel='stylesheet/stylus' scoped>
  .wraper
    width 100%
    height 100%
    overflow  hidden
    #thumsCanvas
      width 100%
      height 100%
      background-color lightblue 
</style>