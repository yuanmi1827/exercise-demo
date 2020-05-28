<template>
  <div></div>
</template>

<script type='text/ecmascript-6'>
  export default {
    data () {
      return {
      }
    },
    mounted() {
      const str= 'asd fgh jkl'
      console.log(this.reverseWords(str))
    },
    methods: {
      //字符串反转
      reverseWords(str) {
        let left = 0
        let right = str.length -1
        let queue = []
        let word = ''
        while(str.charAt(left) === ' ') left++
        while(str.charAt(right) === ' ') right --
        while(left <= right) {
          let char = str.charAt(left)
          if(char === ' ' && word) {
            queue.unshift(word)
            word = ''
          } else if(char !== ' '){
            word += char
          }
          left ++
        } 
        queue.unshift(word)
        return queue.join(' ')
      }
    }
  }
</script>

<style lang='stylus' rel='stylesheet/stylus' scoped>

</style>