<template>
  <div>
    <!--<div class="vux-demo">-->
      <!--<img class="logo" src="../assets/vux_logo.png">-->
      <!--<h1></h1>-->
    <!--</div>-->
    <!--<group title="cell demo">-->
      <!--<cell title="Vux" value="Cool" is-link></cell>-->
      <!--<cell title="Vux" value="Cool" is-link></cell>-->
    <!--</group>-->

    <scroller lock-x height="1400px" @on-scroll="onScroll">
     <div>
       <search></search>
       <panel header="图文组合列表" :list="list"></panel>
     </div>
    </scroller>


    <!--<scroller lock-x height="400px">-->
    <!--<div>-->
      <!--<p v-for="i in 100">{{i}}</p>-->
    <!--</div>-->
    <!--</scroller>-->

    <!--<group :title="$t('isLink is set to true when link exists')">-->
      <!--<cell :title="$t('Go to Radio Demo')" link="/component/radio" inline-desc='link="/component/radio"'></cell>-->
      <!--<cell :title="$t('Go to Demo')" :link="{path:'/demo'}" inline-desc=':link={path:"/demo"}'></cell>-->
      <!--<cell Ltitle="$t('http link')" link="https://vux.li" inline-desc='link="https://vux.li"'></cell>-->
    <!--</group>-->

    <TabbarFooter></TabbarFooter>


  </div>
</template>

<script>
import { Group, Cell ,Panel,Scroller,Search} from 'vux'
import TabbarFooter from './TabbarFooter.vue'

export default {
  components: {
    Group,
    Cell,
    TabbarFooter,
    Panel,
    Scroller,
    Search
  },
  methods: {
    onScroll (pos) {
      console.log('on scroll', pos)
      this.scrollTop = pos.top
    }
  },
  data () {
    return {
      list: [
      {
        title: '标题一',
        desc: '由各种物质组成的巨型球状天体，叫做星球。星球有一定的形状，有自己的运行轨道。',
        url: '/component/cell'
      },
      {
        title: '标题一',
        desc: '由各种物质组成的巨型球状天体，叫做星球。星球有一定的形状，有自己的运行轨道。',
        url: '/component/cell'
      },
      {
        title: '标题一',
        desc: '由各种物质组成的巨型球状天体，叫做星球。星球有一定的形状，有自己的运行轨道。',
        url: '/component/cell'
      },
      {
        title: '标题一',
        desc: '由各种物质组成的巨型球状天体，叫做星球。星球有一定的形状，有自己的运行轨道。',
        url: '/component/cell'
      },
      {
        src: 'http://placeholder.qiniudn.com/60x60/3cc51f/ffffff',
        title: '标题二',
        desc: '由各种物质组成的巨型球状天体，叫做星球。星球有一定的形状，有自己的运行轨道。',
        url: {
          path: '/component/radio',
          replace: false
        }
      },
      {
        src: 'http://placeholder.qiniudn.com/60x60/3cc51f/ffffff',
        title: '标题二',
        desc: '由各种物质组成的巨型球状天体，叫做星球。星球有一定的形状，有自己的运行轨道。',
        url: {
          path: '/component/radio',
          replace: false
        }
      }],
    }
  }
}

</script>

<style>

</style>
