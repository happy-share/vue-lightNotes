<template>
    <div>
      <mt-tabbar>
        <mt-tab-item id="外卖">
          <img slot="icon" src="../assets/100x100.png">
          外卖
        </mt-tab-item>
        <mt-tab-item id="订单">
          <img slot="icon" src="../assets/100x100.png">
          订单
        </mt-tab-item>
        <mt-tab-item id="发现">
          <img slot="icon" src="../assets/100x100.png">
          发现
        </mt-tab-item>
        <mt-tab-item id="我的">
          <img slot="icon" src="../assets/100x100.png">
          我的
        </mt-tab-item>
      </mt-tabbar>
    </div>
</template>
<script>
export default {
  name: 'tabbar',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>
