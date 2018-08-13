f<template>
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
      <div class="page__intro">
        <p>
          We’ve curated an adventure that takes you from Hanoi - the bustling heart of Vietnam, through the peaceful rice fields in Yen Bai, up into Ha Giang’s breathtaking mountains, across the stunning Ma Pi Leng Pass, and back down past beautiful Ba Be Lake. Along the way, you will experience unmatched Vietnamese hospitality, try deliciously unique food (and plenty of rice wine), and see landscapes that can’t be beat. In 8 days, we will cover almost 1,000 kilometers. This journey is not for the faint-hearted, but you’ll see why we came here and never left.
        </p>
        <div class="button__wrapper">
          <a target="_blank" href="https://drive.google.com/file/d/1OoKRnvGJobL-cSTRhCJY5_3UGoT1s8-4/view" class="button-link" to="/tours"><span>View Detailed Itinerary</span></a>
        </div>
      </div>
      <main>
        <DetailsTable/>
        <div class="table__image">
          <img src="https://scontent.fmex5-1.fna.fbcdn.net/v/t1.0-9/38615045_1973420626073535_8959041208085118976_n.jpg?_nc_cat=0&oh=174a3c9aadb9aa33b46b397abd9040e7&oe=5BC62432">
        </div>
      </main>
      <Article/>
    </section>
    <div class="banner">
      <h3>Additional Information</h3>
      <p>Vietnam is one of the cheapest countries in the world. You can bring money over in USD and we will help you exchange it for Dong or you can activate your bank account in Vietnam. Just be aware that once we leave the city there are very few ATMS.
  For a 1 week tour we would recommend bringing between $200 and $300. That would cover plenty of beer, coffee and some souvenirs.
      </p>
    </div>
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
    margin:4rem 0 2rem;
    opacity:.8;
  }

  h3 {
    color:#fff;
    text-align:center;
    margin-bottom:.8rem;
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

  .page__intro p {
    margin: 0 2rem 2rem;
    font-size: .9rem;
    line-height: 1.4rem;
  }

  .page-hero__content {
    flex:3;
    align-items:center;
    display:flex;
  }

  section > main {
    display:flex;
  }

  .table__image {
    flex: 1;
    width: 100%;
    margin: 1rem;

    & img {
      object-fit: cover;
      object-position: center;
      width: 100%;
      height: 100%;
    }
  }

  .banner {
    background-color:#3f46ad;
    color:#fff;
    width:100%;
    padding:1rem 3rem 3rem;

    & p {
      font-size: .9rem;
    }
  }

  .button__wrapper {
    display:flex;
    align-items:center;
    justify-content:center;
    margin-bottom:2rem;
  }

</style>


