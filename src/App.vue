<template>
  <div id="app">
    <router-view />
    <tab-bar>
      <tab-bar-item path="/home" activeColor="pink">
        <img slot="item-icon" src="@/assets/img/tabbar/home.png" />
        <img
          slot="item-icon-active"
          src="@/assets/img/tabbar/home_active.png"
        />
        <div slot="item-text">首页</div>
      </tab-bar-item>
      <tab-bar-item path="/category" activeColor="blue">
        <img slot="item-icon" src="@/assets/img/tabbar/category.png" />
        <img
          slot="item-icon-active"
          src="@/assets/img/tabbar/category_active.png"
        />
        <div slot="item-text">分类</div>
      </tab-bar-item>
      <tab-bar-item path="/shopCart" activeColor="pink">
        <img slot="item-icon" src="@/assets/img/tabbar/shopcart.png" />
        <img
          slot="item-icon-active"
          src="@/assets/img/tabbar/shopcart_active.png"
        />
        <div slot="item-text">购物车</div>
      </tab-bar-item>
      <tab-bar-item path="/profile" activeColor="blue">
        <img slot="item-icon" src="@/assets/img/tabbar/profile.png" />
        <img
          slot="item-icon-active"
          src="@/assets/img/tabbar/profile_active.png"
        />
        <div slot="item-text">我的</div>
      </tab-bar-item>
    </tab-bar>
  </div>
</template>

<script>
import TabBar from "@/components/tabbar/TabBar";
import TabBarItem from "@/components/tabbar/TabBarItem";
export default {
  name: "App",
  components: {
    TabBar,
    TabBarItem,
  }
};
</script>

<style>
@import "./assets/css/base";
</style>
