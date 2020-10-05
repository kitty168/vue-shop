<template>
  <div>
    后台首页
    <el-button type="primary" size="default" @click="logout">退出登录</el-button>
  </div>
</template>

<script>
export default {
  methods: {
    logout () {
      window.sessionStorage.clear()
      this.$router.push('/login')
    }
  }
}
</script>

<style lang="less" scoped>
</style>
