<template>
  <div class="home">
    <el-container>
      <el-aside width="200px">
        <home-aside></home-aside>
      </el-aside>
      <el-container>
        <el-header>
          <home-header></home-header>
        </el-header>
        <el-main>Main</el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
import HomeHeader from './components/HomeHeader'
import HomeAside from './components/HomeAside'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeAside
  }
}
</script>

<style lang="stylus" scoped>
  .home
    margin: 0
    position absolute
    width: 100%
    height: 100%
    overflow: hidden
    padding-top: 0
    .el-container
      width: 100%;
      height: 100%;
    .el-header, .el-footer {
      background-color: #545c64;
      color: #333;
      text-align: center;
      line-height: 60px;
    }

    .el-aside {
      position: relative
      background-color: #545c64;
      color: #333;
      text-align: center;
      line-height: 200px;
    }

    .el-main {
      background-color: #E9EEF3;
      color: #333;
      text-align: center;
      line-height: 160px;
    }

    body > .el-container {
      margin-bottom: 40px;
    }

    .el-container:nth-child(5) .el-aside,
    .el-container:nth-child(6) .el-aside {
      line-height: 260px;
    }

    .el-container:nth-child(7) .el-aside {
      line-height: 320px;
    }
</style>
