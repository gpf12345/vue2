<template>
  <div>

    <!-- 这是二级路由出口 -->
     <router-view></router-view>
    <van-tabbar route active-color="#ee0a24" inactive-color="#000" v-model="active">
      <van-tabbar-item to="/home" icon="home-o">首页</van-tabbar-item>
      <van-tabbar-item to="/category" icon="apps-o">分类页</van-tabbar-item>
      <van-tabbar-item to="/cart" icon="shopping-cart-o">购物车</van-tabbar-item>
      <van-tabbar-item to="/user" icon="user-o">我的</van-tabbar-item>
    </van-tabbar>
  </div>
</template>

<script>
export default {
  name: 'MyLayout',
  data () {
    return {
      active: 'home'
    }
  }
}
</script>
