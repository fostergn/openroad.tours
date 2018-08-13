f<template>
  <main>
    <section class="hero">
      <div class="image__wrapper">
        <img src="https://scontent.fmex5-1.fna.fbcdn.net/v/t1.0-9/31277625_1818007854948147_8930219885879885824_o.jpg?_nc_cat=0&oh=5680c125a56aa7aaaed66e0b623fa099&oe=5BC9A3DE" alt="">
      </div>
      <div class="page-hero__content">
        <TailormadePageHeroContent />
      </div>
    </section>
    <section>
      <header>
        <h2>We Cater To Your Needs</h2>
      </header>
      <div class="page__intro">
        <p>
          We’ve curated an adventure that takes you from Hanoi - the bustling heart of Vietnam, through the peaceful rice fields in Yen Bai, up into Ha Giang’s breathtaking mountains, across the stunning Ma Pi Leng Pass, and back down past beautiful Ba Be Lake. Along the way, you will experience unmatched Vietnamese hospitality, try deliciously unique food (and plenty of rice wine), and see landscapes that can’t be beat. In 8 days, we will cover almost 1,000 kilometers. This journey is not for the faint-hearted, but you’ll see why we came here and never left.
        </p>
      </div>
      <SecondaryContent
        headerContent="Tell Us What You Have In Mind"
        sidebarContent=""
        formHeader=""
      />
    </section>
  </main>
</template>

<script>
  import TailormadePageHeroContent from '@/components/TailormadePageHeroContent'
  import DetailsTable from '@/components/DetailsTable'
  import Article from '@/components/Article'
  import SecondaryContent from '@/components/SecondaryContent'

  export default {
    components: {
      TailormadePageHeroContent,
      DetailsTable,
      Article,
      SecondaryContent
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

</style>
