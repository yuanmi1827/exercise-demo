<template>
  <div class="Box">
    <div class="title">被扫架构图<div class="title-bg"></div></div>
    <div class="container-box">
      <ul class="list-ul">
        <li class="list-item">
          <div class="desc-info">
            <span></span>
            <span class="circle"></span>
            <span class="text">客户码</span>
            <span class="text"></span>
          </div>
          <div class="line1">
            <div class="line1-animate"></div>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" @click="goArchitecture('聚合支付被扫 - APIP - API开放平台','外高桥','APIP')"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">APIP</span>
            <span class="text">API开放平台</span>
          </div>
          <div class="line2 left" style="transform:rotate(-30deg)">
            <div class="line2-animate"></div>
          </div>
          <div class="line3 left" style="transform:rotate(-16deg)">
            <div class="line3-animate"></div>
          </div>
          <div class="line4 left" style="transform:rotate(17deg)">
            <div class="line4-animate"></div>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" @click="goArchitecture('聚合支付被扫 - SAES收单业务','外高桥','SAES')">
            <span class=""></span> 
            <span class="circle"></span> 
            <span class="text">SAES</span>
            <span class="text">收单业务</span>
          </div>
          <div class="line5 left" style="transform:rotate(-52deg)">
            <div class="line5-animate"></div>
          </div>
          <div class="line6 left" style="transform:rotate(-21deg)">
            <div class="line6-animate"></div>
          </div>
          <div class="line7 left" style="transform:rotate(-16deg)">
            <div class="line7-animate"></div>
          </div>
          <div class="line8 left" style="transform:rotate(-10deg)">
            <div class="line8-animate"></div>
          </div>
           <div class="line9 left" style="transform:rotate(0deg)">
            <div class="line9-animate"></div>
          </div>
          <div class="line10 left" style="transform:rotate(17deg)">
            <div class="line10-animate"></div>
          </div>
          <div class="line-col">
            <div class="linecol-animate"></div>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" @click="goArchitecture('聚合支付被扫 - CCAP商业卡收单','外高桥','CCAP')"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">CCAP</span>
            <span class="text">商业卡收单</span>
          </div>
           <div class="line11 left" style="transform:rotate(17deg)">
            <div class="line11-animate"></div>
          </div>
          <div class="line12 left" style="transform:rotate(52deg)">
            <div class="line12-animate"></div>
          </div>
          <div class="line-col">
            <div class="linecol-animate"></div>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" @click="goArchitecture2('聚合支付被扫 - BOOM卡组织支付','外高桥','BOOM')"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">BOOM</span>
            <span class="text">卡组织支付</span>
          </div>
          <div class="line13 left" style="transform:rotate(-17deg)">
            <div class="line13-animate"></div>
          </div>
          <div class="line14 left" style="transform:rotate(40deg)">
            <div class="line14-animate"></div>
          </div>
          <div class="line-col">
            <div class="linecol-animate"></div>
          </div>
        </li>
      </ul>
      <ul class="list-ul">
        <li class="list-item">
          <div class="desc-info" v-show="false"> 
            <span></span>
            <span class="circle"></span>
            <span class="text"></span>
            <span class="text"></span>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">商户之家扫码</span>
            <span class="text"></span>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" v-show="false"> 
            <span></span>
            <span class="circle"></span>
            <span class="text"></span>
            <span class="text"></span>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" v-show="false"> 
            <span></span>
            <span class="circle"></span>
            <span class="text"></span>
            <span class="text"></span>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" @click="goArchitecture('聚合支付被扫 - OFST电子商务交易中心','外高桥','OFST')"> 
            <span></span>
            <span class="text">OFST</span>
            <span class="text">电子商务</span>
            <span class="text">交易中心</span>
          </div>
        </li>
      </ul>

      <ul class="list-ul">
        <li class="list-item">
          <div class="desc-info"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">POSC</span>
            <span class="text">商户终端</span>
          </div>
        </li>
        <li class="list-item" style="height:1.5rem">
          <div class="desc-info" v-show="false"> 
            <span></span>
            <span class="circle"></span>
            <span class="text"></span>
            <span class="text"></span>
          </div>
          <div class="line15" style="transform:rotate(64deg)">
            <div class="line15-animate"></div>
          </div>
          <div class="line-colcenter">
            <div class="linecolcenter-animate"></div>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" @click="goArchitecture('聚合支付被扫 - BIFS综合前置','西三旗','BIFS')"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">BIFS</span>
            <span class="text">综合前置</span>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info"> 
            <span></span>
            <span class="circle" v-show="false"></span>
            <span class="text"></span>
            <span class="text"></span>
          </div>
        </li>
        <li class="list-item" style="height:3.5rem">
          <div class="desc-info" v-show="false"> 
            <span></span>
            <span class="circle"></span>
            <span class="text"></span>
            <span class="text"></span>
          </div>
        </li>
        <li class="list-item" style="height:2.5rem">
          <div class="desc-info"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">银联</span>
            <span class="text"></span>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">微信/支付宝</span>
            <span class="text"></span>
          </div>
          <div class="line-col">
            <div class="linecol-animate"></div>
          </div>
        </li>
      </ul>

      <ul class="list-ul">
        <li class="list-item">
          <div class="desc-info" v-show="false"> 
            <span></span>
            <span class="circle"></span>
            <span class="text"></span>
            <span class="text"></span>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">商户之家扫码</span>
            <span class="text"></span>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" @click="goArchitecture('聚合支付被扫 - BIFS综合前置','嘉定','BIFS')"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">BIFS</span>
            <span class="text">综合前置</span>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" v-show="false"> 
            <span></span>
            <span class="circle"></span>
            <span class="text"></span>
            <span class="text"></span>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" @click="goArchitecture('聚合支付被扫 - OFST电子商务交易中心','嘉定','OFST')"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">OFST</span>
            <span class="text">电子商务</span>
            <span class="text">交易中心</span>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" v-show="false"> 
            <span></span>
            <span class="circle"></span>
            <span class="text"></span>
            <span class="text"></span>
          </div>
        </li>
      </ul>

      <ul class="list-ul">
        <li class="list-item">
          <div class="desc-info"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">商户扫码</span>
            <span class="text"></span>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" @click="goArchitecture('聚合支付被扫 - APIP - API开放平台','嘉定','APIP')"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">APIP</span>
            <span class="text">API开放平台</span>
          </div>
          <div class="line2 right" style="transform:rotate(210deg)">
            <div class="line2-animate"></div>
            <div class="line2-animate"></div>
          </div>
          <div class="line-col">
            <div class="linecol-animate"></div>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" @click="goArchitecture('聚合支付被扫 - SAES收单业务','嘉定','SAES')"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">SAES</span>
            <span class="text">收单业务</span>
          </div>
          <div class="line5 right" style="transform:rotate(233deg)">
            <div class="line5-animate"></div>
          </div>
          <div class="line6 right" style="transform:rotate(201deg)">
            <div class="line6-animate"></div>
          </div>
          <div class="line8 right" style="transform:rotate(-170deg)">
            <div class="line8-animate"></div>
          </div>
          <div class="line10 right" style="transform:rotate(163deg)">
            <div class="line10-animate"></div>
          </div>
          <div class="line16 right" style="transform:rotate(180deg)">
            <div class="line16-animate"></div>
          </div>
          <div class="line-col">
            <div class="linecol-animate"></div>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" @click="goArchitecture('聚合支付被扫 - CCAP商业卡收单','嘉定','CCAP')"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">CCAP</span>
            <span class="text">商业卡收单</span>
          </div>
          <div class="line-col">
            <div class="linecol-animate"></div>
          </div>
          <div class="line12 right" style="transform:rotate(126deg)">
            <div class="line12-animate"></div>
          </div>
        </li>
        <li class="list-item">
          <div class="desc-info" @click="goArchitecture2('聚合支付被扫 - BOOM卡组织支付','嘉定','BOOM')"> 
            <span></span>
            <span class="circle"></span>
            <span class="text">BOOM</span>
            <span class="text">卡组织支付</span>
          </div>
          <div class="line-col">
            <div class="linecol-animate"></div>
          </div>
          <div class="line14 right" style="transform:rotate(140deg)">
            <div class="line14-animate"></div>
          </div>
        </li>
      </ul>         
    </div>
    <div class="box-left">外高桥</div>
    <div class="box-center">西三旗</div>
    <div class="box-right">嘉定</div>
  </div>
</template>

<script>
export default {
  name: 'Architecture',
  components: {
  
  },
  data () {
    return {
      yichang: [{code: 1, name: ['CCAP']},{code:3, name: ['CCAP','SAES']}]
    }
  },
  methods:{
    // 跳转架构图节点详情页
    goArchitecture(appName,region,appEnName) {
      // console.log(appName,region,appEnName,'88888888888')
      this.$router.push({path:'/architectureOne',query:{
        appName: appName,      
        region: region,         // 地区
        appEnName: appEnName,
        idFlag: 'A2'
      }})
    },
    // 跳转架构图GTCG/BOOM节点详情页
    goArchitecture2(appName,region,appEnName) {
      // console.log(appName,region)
      this.$router.push({path:'/architectureTwo',query:{
        appName: appName,      
        region: region,         // 地区
        appEnName: appEnName,
        idFlag: 'A2'
      }})
    },
    getAllClass() {
      this.yichang.forEach((item) => {
        if(item.code === 1) {
          for(let i=0;i<(document.getElementsByClassName('list-ul').length-3);i++) {
            for(let j=0;j<document.getElementsByClassName('list-ul')[i].children.length;j++){
              for(let k=0;k<document.getElementsByClassName('list-ul')[i].children[j].children[0].children.length;k++){
                item.name.forEach((item2) => {
                  if(document.getElementsByClassName('list-ul')[i].children[j].children[0].children[k].innerHTML===item2){
                    this.addClass(document.getElementsByClassName('list-ul')[i].children[j].children[0].children[0],'radius')
                    this.addClass(document.getElementsByClassName('list-ul')[i].children[j].children[0].children[1],'redColor')
                  }
                })
              }
            }
          }
        } else if(item.code === 2){
          for(let j=0;j<document.getElementsByClassName('list-ul')[2].children.length;j++){
            for(let k=0;k<document.getElementsByClassName('list-ul')[2].children[j].children[0].children.length;k++){
              item.name.forEach((item2) => {
                if(document.getElementsByClassName('list-ul')[2].children[j].children[0].children[k].innerHTML===item2){
                  this.addClass(document.getElementsByClassName('list-ul')[2].children[j].children[0].children[0],'radius')
                  this.addClass(document.getElementsByClassName('list-ul')[2].children[j].children[0].children[1],'redColor')
                }
              })
            }
          }
        } else {
          for(let i=4;i<(document.getElementsByClassName('list-ul').length);i++) {
            for(let j=0;j<document.getElementsByClassName('list-ul')[i].children.length;j++){
              for(let k=0;k<document.getElementsByClassName('list-ul')[i].children[j].children[0].children.length;k++){
                item.name.forEach((item2) => {
                  if(document.getElementsByClassName('list-ul')[i].children[j].children[0].children[k].innerHTML===item2){
                    this.addClass(document.getElementsByClassName('list-ul')[i].children[j].children[0].children[0],'radius')
                    this.addClass(document.getElementsByClassName('list-ul')[i].children[j].children[0].children[1],'redColor')
                  }
                })
              }
            }
          }
        }
      })
    },
    hasClass(el, className) {
      let reg = new RegExp('(^|\\s)' + className + '(\\s|$)')
      return reg.test(el.className)
    },
    addClass(el, className) {
      if (this.hasClass(el, className)) {
        return
      }
      let newClass = el.className.split(' ')
      newClass.push(className)
      el.className = newClass.join(' ')
    },
    unip(el,className) {
      el.remove(className)
    }
  },
  mounted() {
    this.getAllClass()
  },
 
}
</script>

<style lang="stylus" scoped>
  px2rem(designpx) {
    $rem=37.5
    return (designpx/$rem)rem
  }
  .Box{
    width 100%
    // height 600px
    box-sizing border-box
    padding 0 px2rem(10) 30px px2rem(10)
    display flex
    flex-direction column
    position relative
    border-top px2rem(6) solid #F2F2F2
    .title{
      margin px2rem(15) 0
      padding px2rem(10) 0
      // margin-bottom px2rem(20)
      font-family PingFangSC-Medium
      font-size px2rem(15)
      color #383838
      // height px2rem(35)
      line-height px2rem(0)
      font-weight bold
      position relative
      .title-bg {
        width px2rem(76)
        height px2rem(8)
        background rgba(35,139,224,0.20)
        position absolute
        bottom 0
      }
    }
    .container-box{
      flex 1
      display flex
      .list-ul{
        width 20%
        display flex
        flex-direction column
        .list-item{
          text-align center
          // flex 1
          height px2rem(80)
          position relative
          .desc-info{
            display flex
            flex-direction column
            align-items center
            position relative
            // justify-content center
            .radius {
              width px2rem(24)
              height px2rem(24)
              border-radius 50%
              background rgba(250,113,95,0.30)
              position absolute
              top px2rem(-6)
            }
            .circle {
              width px2rem(12)
              height px2rem(12)
              border-radius 50%
              background-color #50D5DE
              &.redColor{
                background-color #fa715f
              }
            }
            .text {
              white-space nowrap
              font-size px2rem(11)
              color #212121
              font-family PingFangSC-Regular
            }
          }
          .line15{
            width px2rem(165)
            height 2px
            background #E7EEFF
            position absolute
            left px2rem(35)
            top px2rem(-65)
            z-index -1
            margin-top -1px
            transform-origin left
            .line15-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(20)
              height 2px
              background-image linear-gradient(270deg,#6767D7 0%,#E7EEFF 100%)
              animation line15 1.5s linear 0s infinite
            }
          }
          .line1{
            width px2rem(120)
            height 2px
            background #E7EEFF
            position absolute
            top px2rem(5)
            left px2rem(45)
            z-index -1
            margin-top -1px
            .line1-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(30)
              height 2px
              background-image linear-gradient(270deg,#6767D7 0%,#E7EEFF 100%)
              animation  line1 1.5s linear 0s infinite
            }
          }
          .line2 {
            width px2rem(145)
            height 2px
            background #E7EEFF
            position absolute
            top px2rem(5)
            z-index -1
            margin-top -1px
            transform-origin left
            .line2-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(30)
              height 2px
              background-image linear-gradient(-270deg,#6767D7 0%,#E7EEFF 100%)
              animation line2 1.5s linear 0s infinite reverse
              // &:nth-child(2) {
              //   background-image linear-gradient(-270deg,#6767D7 0%,#E7EEFF 100%)
              //   animation line2 1.5s linear 0s infinite reverse
              // }
            }
          }
          .line3 {
            width px2rem(275)
            height 2px
            background #E7EEFF
            position absolute
            top px2rem(5)
            z-index -1
            margin-top -1px
            transform-origin left
            .line3-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(40)
              height 2px
              background-image linear-gradient(-270deg,#6767D7 0%,#E7EEFF 100%)
              animation line3 1.5s linear 0s infinite reverse
            }
          }
          .line4 {
            width px2rem(280)
            height 2px
            background #E7EEFF
            position absolute
            top px2rem(5)
            z-index -1
            margin-top -1px
            transform-origin left
            .line4-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(40)
              height 2px
              background-image linear-gradient(270deg,#6767D7 0%,#E7EEFF 100%)
              animation line4 1.5s linear 0s infinite
            }
          }
          .line-col{
            width px2rem(60)
            height 2px
            background #E7EEFF
            position absolute
            left px2rem(5)
            top px2rem(-35)
            z-index -1
            margin-top -1px
            transform rotate(90deg)
            .linecol-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(20)
              height 2px
              background-image linear-gradient(270deg,#6767D7 0%,#E7EEFF 100%)
              animation linecol-animate 1.5s linear 0s infinite
            }
          }
          .line-colcenter{
            width px2rem(120)
            height 2px
            background #E7EEFF
            position absolute
            left px2rem(-24)
            top px2rem(-5)
            z-index -1
            margin-top -1px
            transform rotate(90deg)
            .linecolcenter-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(20)
              height 2px
              background-image linear-gradient(270deg,#6767D7 0%,#E7EEFF 100%)
              animation linecolcenter-animate 1.5s linear 0s infinite
            }
          }
          .line5 {
            width px2rem(95)
            height 2px
            background #E7EEFF
            // background red
            position absolute
            top px2rem(5)
            z-index -1
            margin-top -1px
            transform-origin left
            .line5-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(20)
              height 2px
              background-image linear-gradient(-270deg,#6767D7 0%,#E7EEFF 100%)
              animation line5 1.5s linear 0s infinite reverse
            }
          }
          .line6 {
            width px2rem(220)
            height 2px
            background #E7EEFF
            // background red
            position absolute
            top px2rem(5)
            z-index -1
            margin-top -1px
            transform-origin left
            .line6-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(20)
              height 2px
              background-image linear-gradient(-270deg,#6767D7 0%,#E7EEFF 100%)
              animation line6 1.5s linear 0s infinite reverse
            }
          }
          .line7 {
            width px2rem(275)
            height 2px
            background #E7EEFF
            // background red
            position absolute
            top px2rem(5)
            z-index -1
            margin-top -1px
            transform-origin left
            .line7-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(20)
              height 2px
              background-image linear-gradient(-270deg,#6767D7 0%,#E7EEFF 100%)
              animation line7 1.5s linear 0s infinite reverse
            }
          }
          .line8 {
            width px2rem(135)
            height 2px
            background #E7EEFF
            // background red
            position absolute
            top px2rem(5)
            z-index -1
            margin-top -1px
            transform-origin left
            .line8-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(20)
              height 2px
              background-image linear-gradient(-270deg,#6767D7 0%,#E7EEFF 100%)
              animation line8 1.5s linear 0s infinite reverse
            }
          } 
          .line9 {
            width px2rem(195)
            height 2px
            background #E7EEFF
            // background red
            position absolute
            top px2rem(5)
            z-index -1
            margin-top -1px
            transform-origin left
            .line9-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(20)
              height 2px
              background-image linear-gradient(-270deg,#6767D7 0%,#E7EEFF 100%)
              animation line9 1.5s linear 0s infinite reverse
            }
          }
          .line10 {
            width px2rem(275)
            height 2px
            background #E7EEFF
            // background red
            position absolute
            top px2rem(5)
            z-index -1
            margin-top -1px
            transform-origin left
            .line10-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(70)
              height 2px
              background-image linear-gradient(270deg,#6767D7 0%,#E7EEFF 100%)
              animation line10 1.5s linear 0s infinite 
            }
          } 
          .line11 {
            width px2rem(275)
            height 2px
            background #E7EEFF
            // background red
            position absolute
            top px2rem(5)
            z-index -1
            margin-top -1px
            transform-origin left
            .line11-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(70)
              height 2px
              background-image linear-gradient(270deg,#6767D7 0%,#E7EEFF 100%)
              animation line11 1.5s linear 0s infinite 
            }
          }  
          .line12 {
            width px2rem(95)
            height 2px
            background #E7EEFF
            // background red
            position absolute
            top px2rem(5)
            z-index -1
            margin-top -1px
            transform-origin left
            .line12-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(20)
              height 2px
              background-image linear-gradient(270deg,#6767D7 0%,#E7EEFF 100%)
              animation line12 1.5s linear 0s infinite 
            }
          }
          .line13 {
            width px2rem(275)
            height 2px
            background #E7EEFF
            // background red
            position absolute
            top px2rem(5)
            z-index -1
            margin-top -1px
            transform-origin left
            .line13-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(70)
              height 2px
              background-image linear-gradient(-270deg,#6767D7 0%,#E7EEFF 100%)
              animation line13 1.5s linear 0s infinite reverse
            }
          }
          .line14 {
            width px2rem(160)
            height 2px
            background #E7EEFF
            // background red
            position absolute
            top px2rem(5)
            z-index -1
            margin-top -1px
            transform-origin left
            .line14-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(20)
              height 2px
              background-image linear-gradient(270deg,#6767D7 0%,#E7EEFF 100%)
              animation line14 1.5s linear 0s infinite 
            }
          }
          .line16 {
            width px2rem(55)
            height 2px
            background #E7EEFF
            // background red
            position absolute
            top px2rem(5)
            z-index -1
            margin-top -1px
            transform-origin left
            .line16-animate{
              position absolute
              top 0
              z-index 0
              width px2rem(20)
              height 2px
              background-image linear-gradient(-270deg,#6767D7 0%,#E7EEFF 100%)
              animation line16 1.5s linear 0s infinite reverse
            }
          }
        }
      }
    }
    .box-left {
      width px2rem(157)
      height px2rem(335)
      border 1px solid #E7EEFF
      position absolute
      top px2rem(100)
      left px2rem(5)
      color #238BE0
      text-align left
      font-size px2rem(11)
      font-family PingFangSC-Regular
      z-index -2
    }
    .box-right {
      width px2rem(157)
      height px2rem(335)
      border 1px solid #E7EEFF
      position absolute
      top px2rem(100)
      right px2rem(5)
      color #238BE0
      text-align right
      font-size px2rem(11)
      font-family PingFangSC-Regular
      z-index -2
    }
    .box-center {
      width px2rem(47)
      height px2rem(335)
      position absolute
      border 1px solid #E7EEFF
      top px2rem(100)
      left 50%
      margin-left px2rem(-23)
      color #238BE0
      text-align center
      font-size px2rem(11)
      font-family PingFangSC-Regular
      z-index -2
    }
  }
  .left {
    left px2rem(45)
  }
  .right {
    left px2rem(25)
  }
  @keyframes line1 {
    from {
      left 0
    }
    to {
      left px2rem(90)
    }
  }
  @keyframes line2 {
    from {
      left 0
    }
    to {
      left px2rem(115)
    }
  }
  
  @keyframes line3 {
    from {
      left 0
    }
    to {
      left px2rem(235)
    }
  }
  @keyframes line4 {
    from {
      left 0
    }
    to {
      left px2rem(240)
    }
  }
  @keyframes line5 {
    from {
      left 0
    }
    to {
      left px2rem(75)
    }
  }
  @keyframes line6 {
    from {
      left 0
    }
    to {
      left px2rem(200)
    }
  }
  @keyframes line7 {
    from {
      left 0
    }
    to {
      left px2rem(255)
    }
  }
  @keyframes line8 {
    from {
      left 0
    }
    to {
      left px2rem(115)
    }
  }
  @keyframes line9 {
    from {
      left 0
    }
    to {
      left px2rem(175)
    }
  }
  @keyframes line10 {
    from {
      left 0
    }
    to {
      left px2rem(205)
    }
  }
  @keyframes line11 {
    from {
      left 0
    }
    to {
      left px2rem(205)
    }
  }
  @keyframes line12 {
    from {
      left 0
    }
    to {
      left px2rem(75)
    }
  }
  @keyframes line13 {
    from {
      left 0
    }
    to {
      left px2rem(205)
    }
  }
  @keyframes line14 {
    from {
      left 0
    }
    to {
      left px2rem(140)
    }
  }
  @keyframes line15 {
    from {
      left 0
    }
    to {
      left px2rem(145)
    }
  }
  @keyframes line16 {
    from {
      left 0
    }
    to {
      left px2rem(35)
    }
  }
  @keyframes linecol-animate {
    from {
      left 0
    }
    to {
      left px2rem(40)
    }
  }
  @keyframes linecolcenter-animate{
    from {
      left 0
    }
    to {
      left px2rem(100)
    }
  }
</style>
