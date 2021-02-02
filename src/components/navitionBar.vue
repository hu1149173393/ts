<template>
<div class="bar">
  <div v-for="(item,index) in array" :key="index">
    <p>{{item.name}}</p>
  </div>
</div>
</template>

<script>
export default {
name: "navitionBar",
  data(){
  return {
    array:[
      {
        name:'个人中心'
      },{
        name:'时间记录'
      },{
        name:'分享经验'
      },{
        name: "一起嗨皮",
      }
    ]
  }
  }
}
</script>

<style scoped lang="less">
.bar{
  width: 100%;
  background: black;
  height: 70px;
  display: flex;
  justify-content: space-between;
}
</style>