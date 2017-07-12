<template>
  <div class="container">
    <div class="navbar-container">
      <el-row>
        <el-col :span="24">
          <el-menu default-active="2" mode="vertical" class="el-menu-vertical-demo">
            <el-submenu index="1">
              <template slot="title">เมนูที่ 1</template>
              <el-menu-item-group title="เมนูย่อยของเมนูที่ 1">
                <el-menu-item index="1-1">เมนูย่อยของเมนูที่ 1-1</el-menu-item>
                <el-menu-item index="1-2">เมนูย่อยของเมนูที่ 1-2</el-menu-item>
              </el-menu-item-group>
            </el-submenu>
            <el-menu-item index="2">เมนูที่ 2</el-menu-item>
            <el-menu-item index="3">เมนูที่ 3</el-menu-item>
          </el-menu>
        </el-col>
      </el-row>
    </div>
    <div class="body-container"><nuxt /></div>
  </div>
</template>

<script>
export default {
}
</script>

<style scoped>
  .container {
    width: 100%;
    height: 100vh;
    background-color: #EEF1F6;
  }
  .navbar-container {
    width: 250px;
    height: 100%;
    float: left;
  }
  .body-container {
    height: 100%;
    background-color: #f9f9f9;
    overflow-y: scroll;
    padding: 10px 40px;
  }
  .languagebar {
    position: absolute;
    bottom: 0px;
    padding: 10px;
  }
</style>
