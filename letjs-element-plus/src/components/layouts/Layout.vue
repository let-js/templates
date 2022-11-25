<template>
  <el-container style="height: 100%">
    <el-header class="header">
      <div class="logo-container">
        <router-link :to="'/'"
          ><img style="height: 40px" src="../../assets/logo.png"
        /></router-link>
      </div>
    </el-header>
    <el-main>
      <router-view></router-view>
    </el-main>
    <el-footer class="footer">I am a naughty footer</el-footer>
  </el-container>
</template>
<style lang="scss" scoped>
.header {
  height: 64px;
  padding-left: 0.8rem;
  display: flex;
  border-bottom: solid rgba(60, 60, 67, 0.12) 1px;
}
.logo-container {
  height: 100%;
  line-height: 100%;
  display: flex;
  align-items: center;
  a {
    height: 40px;
  }
}
.footer {
  height: 40px;
  line-height: 40px;
  text-align: center;
  font-size: 1rem;
  bottom: 0;
}
</style>
