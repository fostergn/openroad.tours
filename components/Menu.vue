<template>
  <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
    <h1 class="title">Open Road Tours</h1>
    <el-submenu index="1">
      <template slot="title">Tours</template>
      <el-menu-item index="1-1">North Vietnam</el-menu-item>
      <el-menu-item index="1-2">Tailormade</el-menu-item>
      <el-menu-item index="1-2">Before You Go</el-menu-item>
    </el-submenu>
    <el-menu-item index="2">Blog</el-menu-item>
    <el-menu-item index="3">Contact</el-menu-item>
  </el-menu>
</template>

<script>
  export default {
    data() {
      return {
        activeIndex: '1',
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<style scoped>
  .title {
    padding:0 14px;
    font-size:1.2rem;
    display: flex;
    align-items: center;
    height:60px;
  }
  .el-menu {
    display:flex;
    align-items:center;
    /*justify-content:flex-end;*/
  }

  li:nth-child(2) {
    margin-left:auto;
  }
</style>
