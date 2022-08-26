<template>
  <div>
    <el-button type="info" @click="logout">退出</el-button>
    <h2>这个是home组件</h2>
  </div>
</template>

<script>
export default {
  methods: {
    logout() {
      window.sessionStorage.clear()
      this.$router.push('/login')
    }
  }
}
</script>

<style lang="less" scoped>
</style>
