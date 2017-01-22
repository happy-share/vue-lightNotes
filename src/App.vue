<template>
  <div>
    <mt-header fixed title="固定在顶部"></mt-header>
    <demo></demo>
    <tabbar></tabbar>
  </div>
</template>

<script>
import Demo from './components/Demo'
import Tabbar from './components/Tabbar'

export default {
  name: 'app',
  components: {
    Demo,
    Tabbar
  }
}

</script>
