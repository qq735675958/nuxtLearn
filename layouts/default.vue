<template>
  <a-layout id="components-layout-demo-top" class="layout">
    <Header></Header>
    <a-layout-content style="padding: 0 50px">
      <div :style="{ background: '#fff', minHeight: '600px' }">
        <Nuxt/>
      </div>
    </a-layout-content>
    <Footer/>
  </a-layout>
</template>

<script>
export default {
  name: 'layoutPage',
  data(){
    return{}
  },
  methods:{
    gogo(){
      this.$router.push('/home')
    }
  }
}
</script>
<style lang="less">
  
</style>
