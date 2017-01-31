<template>
  <div>
    <search @result-click="resultClick" @on-change="getResult" :results="results" v-model="value"></search>
    <h1>搜索：查找笔记，URL或标签</h1>
    <TabbarFooter></TabbarFooter>
  </div>
</template>
<style>

</style>
<script>
  import { Search} from 'vux'
  import TabbarFooter from './TabbarFooter.vue'


  export default{
      components:{
          Search,
          TabbarFooter
      },
      methods: {
        resultClick (item) {
          window.alert('you click the result item: ' + JSON.stringify(item))
        },
        getResult (val) {
          this.results = val ? getResult(this.value) : []
        }
      },
      data () {
        return {
          results: [],
          value: ''
        }
      }
  }

  function getResult (val) {
      let rs = []
      for (let i = 0; i < 8; i++) {
        rs.push({
          title: `${val} result: ${i + 1} `,
          other: i
        })
      }
      return rs
  }

</script>
