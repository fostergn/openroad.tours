<template>
  <div>
    <Menu />
    Tours my dude
    <nuxt-child/>
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
