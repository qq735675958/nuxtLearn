<!-- Please remove this file from your project -->
<template>
  <a-layout-header class="header-box">
    <div class="logo">logo</div>
    <a-menu v-model="current" mode="horizontal" @click="change">
      <a-menu-item key="mail"> Navigation One </a-menu-item>
      <a-menu-item key="app"> Navigation Two </a-menu-item>
      <a-sub-menu key="setting">
        <span slot="title" class="submenu-title-wrapper"
          >Navigation Three - Submenu</span
        >
        <a-menu-item-group>
          <a-menu-item key="setting:1">
            Option 1
          </a-menu-item>
          <a-menu-item key="setting:2">
            Option 2
          </a-menu-item>
          <a-menu-item key="setting:3">
            Option 3
          </a-menu-item>
          <a-menu-item key="setting:4">
            Option 4
          </a-menu-item>
        </a-menu-item-group>
      </a-sub-menu>
      <a-menu-item key="alipay">
        <a href="https://antdv.com" target="_blank" rel="noopener noreferrer"
          >Navigation Four - Link</a
        >
      </a-menu-item>
    </a-menu>
  </a-layout-header>
</template>

<script>
export default {
  name: 'Header',
  data(){
    return{
      current: ['setting'],
    }
  },
  methods:{
    change({ item, key, keyPath }){
      console.log(item)
       console.log(key)
        console.log(keyPath)
    }
  }
}
</script>

<style lang="less">
.ant-layout-header{
  background: #fff;
  height: 60px;
  border-bottom: 1px solid rgba(255,255,255,0.8);
}
#components-layout-demo-top .logo {
    width: 120px;
    height: 31px;
    background: #001529;
    margin: 16px 24px 16px 0;
    float: left;
    line-height: 31px;
    color: #fff;
    text-align: center;
  }
  .header-box{
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
</style>
