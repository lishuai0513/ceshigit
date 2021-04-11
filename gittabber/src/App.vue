<template>
  <div id="app">
    <Tabbar>
      <TabbarItem path='/home' activeColor='blue'> 
        <img slot="item-img" src="@/assets/img/tabbar/首页.png" alt="" />
        <img slot="item-img-active" src="@/assets/img/tabbar/首页1.png" alt="" />
        <div slot="item-txt">首页</div>
      </TabbarItem>
      <TabbarItem path='/category'>
        <img slot="item-img" src="@/assets/img/tabbar/分类.png" alt="" />
        <img slot="item-img-active" src="@/assets/img/tabbar/分类1.png" alt="" />
        <div slot="item-txt">分类</div>
      </TabbarItem>
      <TabbarItem path='/cart'>
        <img slot="item-img" src="@/assets/img/tabbar/购物车.png" alt="" />
        <img slot="item-img-active" src="@/assets/img/tabbar/购物车1.png" alt="" />
        <div slot="item-txt">购物车</div>
      </TabbarItem>
      <TabbarItem path='/profile'>
        <img slot="item-img" src="@/assets/img/tabbar/我的.png" alt="" />
        <img slot="item-img-active" src="@/assets/img/tabbar/我的1.png" alt="" />
        <div slot="item-txt">我的</div>
      </TabbarItem>
    </Tabbar>
    <router-view></router-view>
  </div>
</template>

<script>
import Tabbar from "./components/tabbar/Tabbar";
import TabbarItem from "./components/tabbar/TabbarItem";
export default {
  components: {
    Tabbar,
    TabbarItem,
  },
};
</script>

<style scoped>
@import "./assets/css/base.css";
</style>
