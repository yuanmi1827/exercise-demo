<template>
  <div>fu
    <zi :value="value"></zi>
  </div>
</template>

<script type='text/ecmascript-6'>
import zi from './zi'
  export default {
    data () {
      return {
        value: 'aaaa'
      }
    },
    mounted() {
      setTimeout(() => {
        this.value = 'yyyy'
      }, 10000)
    },
    components: {
      zi
    }
  }
</script>

<style lang='stylus' rel='stylesheet/stylus' scoped>

</style>