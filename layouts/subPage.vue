<template>
  <div>
    <Nuxt/>
  </div>
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
