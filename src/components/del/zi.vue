<template>
  <div>zi</div> 
</template>

<script type='text/ecmascript-6'>
  export default {
    props: {
      value: {
        type: String
      }
    },
    data () {
      return {
      }
    },
    watch: {
      value(newVal) {
        this.value = newVal
        console.log(newVal)
      }
    }
  }
</script>

<style lang='stylus' rel='stylesheet/stylus' scoped>

</style>