<template>
  <el-menu :router="true" :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
    <h1 class="title"><nuxt-link to="/">Open Road Tours</nuxt-link></h1>
    <el-submenu index="/tours/north-vietnam">
      <template slot="title"><nuxt-link to="/tours/north-vietnam">Tours</nuxt-link></template>
      <el-menu-item index="/tours/north-vietnam"><nuxt-link to="/tours/north-vietnam">North Vietnam</nuxt-link></el-menu-item>
      <el-menu-item index="/tours/tailormade"><nuxt-link to="/tours/tailormade">Tailormade</nuxt-link></el-menu-item>
      <el-menu-item index="/tours/general-info"><nuxt-link to="/tours/general-info">Before You Go</nuxt-link></el-menu-item>
    </el-submenu>
    <el-menu-item index="/blog" ><nuxt-link to="/blog">Blog</nuxt-link></el-menu-item>
    <el-menu-item index="/about" ><nuxt-link to="/about">Who We Are</nuxt-link></el-menu-item>
    <el-menu-item index="/#contact"><nuxt-link to="/contact">Contact Us</nuxt-link></el-menu-item>
  </el-menu>
</template>

<script>
  export default {
    data() {
      return {
        activeIndex: this.$route.path,
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
  .el-menu {
    border-bottom:none;
  }
  .title {
    padding:0 14px;
    font-size:1.2rem;
    display: flex;
    align-items: center;
    height:60px;
    cursor:pointer;
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
