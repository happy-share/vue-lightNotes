<template>
    <div>
      <tabbar>
        <tabbar-item link="/">
          <img slot="icon" src="../assets/demo/icon_nav_button.png">
          <span slot="label">笔记</span>
        </tabbar-item>
        <tabbar-item show-dot link="/search">
          <img slot="icon" src="../assets/demo/icon_nav_msg.png">
          <span slot="label">搜索</span>
        </tabbar-item>
        <tabbar-item link="/add">
          <img slot="icon" src="../assets/demo/icon_nav_article.png">
          <span slot="label">添加</span>
        </tabbar-item>
        <tabbar-item badge="2" link="/">
          <img slot="icon" src="../assets/demo/icon_nav_cell.png">
          <span slot="label">ＵＲＬ</span>
        </tabbar-item>
      <tabbar-item badge="2" link="/user">
          <img slot="icon" src="../assets/demo/icon_nav_cell.png">
          <span slot="label">账户</span>
        </tabbar-item>
      </tabbar>
    </div>
</template>
<style>
</style>
<script>
import {Tabbar, TabbarItem } from 'vux'

export default {
  components: {
    Tabbar,
    TabbarItem
  },
  data () {
    return {
    }
  }
}
</script>
