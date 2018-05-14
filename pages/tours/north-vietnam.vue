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
    <section>
      <header>
        <h2>General Touring Information</h2>
      </header>
      <main>
        <DetailsTable/>
        <Article/>
      </main>
    </section>
  </main>
</template>

<script>
  import PageHeroContent from '@/components/PageHeroContent'
  import DetailsTable from '@/components/DetailsTable'
  import Article from '@/components/Article'

  export default {
    components: {
      PageHeroContent,
      DetailsTable,
      Article
    }
  }
</script>

<style lang="scss" scoped>

  .hero {
    display:flex;

  }

  h2 {
    font-size:2rem;
    text-align:center;
    margin:4rem 0 3rem;
    opacity:.8;
  }

  .image__wrapper {
    flex:5;
    & >img {
       max-width:100%;
      clip-path: polygon(
        0 0,
        100% 0,
        94% 100%,
        0 100%
      )
    }
  }

  .page-hero__content {
    flex:3;
    align-items:center;
    display:flex;
  }

  section > main {
    display:flex;
  }


</style>


