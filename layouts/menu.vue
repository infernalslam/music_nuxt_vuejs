<template>
  <div class="container">
    <div class="navbar-container">
      <el-row>
        <el-col :span="24">
          <img class="img-logo" src="~assets/img/sellsuki.png" />
          <el-menu  mode="vertical" class="el-menu-vertical-demo">
            <el-submenu index="1">
              <template slot="title">Working</template>
              <el-menu-item-group title="รายการ">
                <el-menu-item index="1-1">งานที่กำลังทำอยู่</el-menu-item>
                <el-menu-item index="1-2">งานที่ทำเสร็จเเล้ว</el-menu-item>
                <el-menu-item index="1-3">Graph Working Flow</el-menu-item>
              </el-menu-item-group>
            </el-submenu>
            <nuxt-link to="/list" class="under-title">
              <el-menu-item index="2">List Working</el-menu-item>
            </nuxt-link>
            <nuxt-link to="/order" class="under-title">
              <el-menu-item index="3">Order Working</el-menu-item>
            </nuxt-link>
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
  .img-logo {
    width: 60%;
    padding-top: 5%;
    text-align: center;
    margin-left: 15%;
  }
  .under-title {
    text-decoration: none;
  }
</style>
