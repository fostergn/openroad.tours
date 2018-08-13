f<template>
  <main>
    <section class="hero">
      <div class="image__wrapper">
        <img src="https://scontent.fmex5-1.fna.fbcdn.net/v/t1.0-9/38030622_1964183196997278_6211474483358728192_n.jpg?_nc_cat=0&oh=a84752f38799ad292dbc208f84ab6857&oe=5C0B1DE8" alt="">
      </div>
      <div class="page-hero__content">
        <ContactPageHeroContent />
      </div>
    </section>
    <section>
      <header>
        <h2>Contact Information</h2>
      </header>
      <div class="page__intro">
        <p class="split-half">
          The motorcycles brought us here, the mountains got us excited, and the people we met along the way kept us coming back. We have combined our passion and know-how to give people the most authentic and unique experiences, in the most beautiful and remote places. We are Open Road Tours.
        </p>
        <p class="split-half">
          The motorcycles brought us here, the mountains got us excited, and the people we met along the way kept us coming back. We have combined our passion and know-how to give people the most authentic and unique experiences, in the most beautiful and remote places. We are Open Road Tours.
        </p>
      </div>
      <SecondaryContent/>
    </section>
  </main>
</template>

<script>
  import ContactPageHeroContent from '@/components/ContactPageHeroContent'
  import SecondaryContent from '@/components/SecondaryContent'

  export default {
    components: {
      ContactPageHeroContent,
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

  .page__intro {
    display:flex;
  }

  .page__intro p {
    margin: 0 2rem 2rem;
    font-size: .9rem;
    line-height: 1.4rem;
    width:50%;
  }

  .page-hero__content {
    flex:3;
    align-items:center;
    display:flex;
  }

  section > main {
    display:flex;
    margin: 0 2rem 2rem;
  }

  section.half {
    width:50%;
  }

  .banner {
    background-color:#3f46ad;
    color:#fff;
    width:100%;
    padding:1rem 3rem 3rem;

    & p {
      font-size: .9rem;
      margin-bottom:1rem;
    }

    a {
      display: block;
      margin: 0 auto;
      width: max-content;
      max-width: 200px;
    }

    a span {
      text-align:center;
      display:block;
      margin:0 auto;
    }
  }

  .header__image {
    width: 200px;
    height: 200px;
    margin:0 auto;

    & img {
      width: 100%;
      height: 100%;
      border-radius: 50%;
      object-fit: cover;
    }
  }

  .half {

    h5 {
      text-align:center;
      margin:1rem 0;
      font-size:1.3rem;
    }

    p {
      font-size:.9rem;
      margin:0 2rem;
    }
  }

</style>


