<template>
  <div>
    <Menu />
    <div class="video__wrapper">
      <div class="video__offset">
        <no-ssr>
          <plyr-youtube id="iIe87ubHQyA" :pe="false" />
        </no-ssr>
      </div>
    </div>
  </div>
</template>

<script>
  import Menu from '@/components/Menu'

  export default {
    components: {
      Menu
    }
  }
</script>

<style lang="scss" scoped>
.video__wrapper {
  clip-path: polygon(0 2%, 100% 0%, 100% 96%, 0 100%);
  position:relative;
  overflow:hidden;
}

.video__offset {
  position:relative;
  top:-8vw;

  &:after {
    content:'';
    width:100%;
    bottom:0;
    position:absolute;
    height:8vw;
    background-color:white;
    z-index:10;
    clip-path: polygon(0% 0%, 100% 13%, 100% 100%, 0 100%);
  }
}
</style>
