<template>
  <Menu />
</template>

<script>
  import Menu from '@/components/Menu'
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
    },
    components: {
      Menu
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
