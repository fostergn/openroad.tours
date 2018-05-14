<template>
  <div class="page__container">
    <Menu/>
    <main>
      <nuxt/>
    </main>
    <Footer/>
  </div>
</template>

<script>
    import Menu from '@/components/Menu'
    import Footer from '@/components/Footer'

    export default {
      components: {
        Menu,
        Footer
      }
    }
</script>

<style lang="scss">
html
*, *:before, *:after
{
  box-sizing: border-box;
  margin: 0;
}

.page {

  &__container {
    overflow:hidden;
    position:relative;
  }
}

main {
  min-height:calc(100vh - 120px)
}

footer {
  min-height:60px;
}
</style>
