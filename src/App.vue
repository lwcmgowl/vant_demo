<template>
  <div id="app">
    <router-view />
    <van-tabbar route v-model="active">
      <van-tabbar-item replace to="/" icon="home-o"> 首页 </van-tabbar-item>
       <van-tabbar-item replace to="/Classify" icon="apps-o"> 分类 </van-tabbar-item>
        <van-tabbar-item replace to="/Find" icon="send-gift-o"> 发现 </van-tabbar-item>
         <van-tabbar-item replace to="/Cart" icon="shopping-cart-o"> 购物车 </van-tabbar-item>
      <van-tabbar-item replace to="/User" icon="user-circle-o">
        我的
      </van-tabbar-item>
    </van-tabbar>
  </div>
</template>
<script>
import { Tabbar, TabbarItem } from 'vant'
export default {
  data () {
    return {
      active: 0
    }
  },
  components: {
    [Tabbar.name]: Tabbar,
    [TabbarItem.name]: TabbarItem
  }
}
</script>
<style lang="scss">
</style>
