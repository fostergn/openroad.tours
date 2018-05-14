<template>
  <main>
    <section class="hero">
      <div class="image__wrapper">
        <img src="https://scontent.fmex6-1.fna.fbcdn.net/v/t1.0-9/26196171_1681996965215904_1718448388478153231_n.jpg?_nc_cat=0&oh=6b934853211937ae8b7d15c486cfb4ca&oe=5B81AC70" alt="">
      </div>
      <div class="page-hero__content">
        <PageHeroContent />
      </div>
    </section>
  </main>
</template>

<script>
  import PageHeroContent from '@/components/PageHeroContent'

  export default {
    components: {
      PageHeroContent
    }
  }
</script>

<style lang="scss" scoped>

  .hero {
    display:flex;

  }

  .image__wrapper {
    flex:5;
    & >img {
       max-width:100%;
    }
  }

  .page-hero__content {
    flex:3;
    align-items:center;
    display:flex;
  }


</style>


