<template>
  <div class="wraper">
    <svg width="375px" height="175px" version="1.1">
      <path fill="transparent" stroke="#FF2851"  id="myPath" stroke-width="4" d="M10 100 L 77 100 T 77 300 L 300 300 "></path>
      <rect x="2" y="-2" width="4" height="4" :stroke="item.color" v-for="(item, index) in rectArr" :key="index">
        <animateMotion dur="6s" :begin="item.delay" repeatCount="indefinite" rotate="auto">
          <mpath xlink:href="#myPath"/>
        </animateMotion>
      </rect>
    </svg>
  </div>
</template>

<script type='text/ecmascript-6'>
export default {
  name: 'one',
  data () {
    return {
      rectArr: [
        {color: 'pink',delay:'0s'},{color: 'pink',delay:'0.05s'},{color: 'pink',delay:'0.1s'},{color: 'pink',delay:'0.15s'},
        {color: 'pink',delay:'0.2'},{color: 'pink',delay:'0.25s'},{color: 'pink',delay:'0.3s'},{color: 'pink',delay:'0.35s'},
        {color: 'pink',delay:'0.4s'},{color: 'pink',delay:'0.45s'},{color: 'pink',delay:'0.5s'},{color: 'pink',delay:'0.55s'},
        {color: 'pink',delay:'0.6s'},{color: 'pink',delay:'0.65s'},{color: 'pink',delay:'0.7s'},{color: 'pink',delay:'0.75s'},
        {color: 'pink',delay:'0.8s'},{color: 'pink',delay:'0.85s'},{color: 'pink',delay:'0.9s'},{color: 'pink',delay:'0.95s'},
      ]
    }
   }
 }
</script>

<style lang='stylus' rel='stylesheet/stylus' scoped>
  .wraper
    width 200%
    height 100%

</style>