<template>
  <div>
    <tab>
      <tab-item :selected="demo1 === '已发货'" @click="demo1 = '已发货'">已发货</tab-item>
      <tab-item :selected="demo1 === '未发货'" @click="demo1 = '未发货'">未发货</tab-item>
      <tab-item :selected="demo1 === '全部订单'" @click="demo1 = '全部订单'">全部订单</tab-item>
    </tab>
    <br/>
    <br/>
    <br/>
    <tab :line-width=2 active-color='#fc378c'>
      <tab-item :selected="demo2 === item" v-for="item in list2" @click="demo2 = item">{{item}}</tab-item>
    </tab>
    <br/>
    <br/>
    <br/>
    <tab :line-width=2>
      <tab-item :selected="demo3 === item" v-for="item in list3" @click="demo3 = item">{{item}}</tab-item>
    </tab>
    <br/>
    <br/>
    <br/>
    <sticky>
      <tab :line-width=1>
      <tab-item :selected="demo4 === item" v-for="item in list4" @click="demo4 = item">{{item}}</tab-item>
      </tab>
    </sticky>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
  </div>
</template>

<script>
  import { Tab, TabItem, Sticky } from '../components/'
  export default {
    components: {
      Tab,
      TabItem,
      Sticky
    },
    data () {
      return {
        demo1: '未发货',
        list2: ['精选', '美食', '电影', '酒店', '外卖'],
        demo2: '美食',
        list3: ['收到的消息', '发出的消息'],
        demo3: '收到的消息',
        list4: ['正在正映', '即将上映'],
        demo4: '即将上映'
      }
    }
  }
</script>