f<template>
  <main>
    <section class="hero">
      <div class="image__wrapper">
        <img src="https://scontent.fmex5-1.fna.fbcdn.net/v/t1.0-9/33380507_1850977604984505_4013360515332964352_o.jpg?_nc_cat=0&oh=860ff99bcd538ee3e62d4a235b80208d&oe=5C043FD1" alt="">
      </div>
      <div class="page-hero__content">
        <AboutPageHeroContent />
      </div>
    </section>
    <section>
      <header>
        <h2>Our Story</h2>
      </header>
      <div class="page__intro">
        <p>
          The motorcycles brought us here, the mountains got us excited, and the people we met along the way kept us coming back. We have combined our passion and know-how to give people the most authentic and unique experiences, in the most beautiful and remote places. We are Open Road Tours.
        </p>
      </div>
      <main>
        <section class="half">
          <header>
            <div class="header__image">
              <img src="https://image.ibb.co/hQ72Vp/Screen_Shot_2018_08_12_at_5_51_18_PM.png">
            </div>
            <h5>Lisa Garsson</h5>
          </header>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vel asperiores quo iusto ipsa quas repellendus enim reiciendis quod sequi, veniam, similique praesentium. Iste vero architecto reprehenderit, nulla veniam mollitia libero.</p>
          <br>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vel asperiores quo iusto ipsa quas repellendus enim reiciendis quod sequi, veniam, similique praesentium. Iste vero architecto reprehenderit, nulla veniam mollitia libero.</p>
        </section>
        <section class="half">
          <header>
            <div class="header__image">
              <img src="https://image.ibb.co/ijoLGU/Screen_Shot_2018_08_12_at_5_53_31_PM.png">
            </div>
            <h5>Eduard Aggenbach</h5>
          </header>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vel asperiores quo iusto ipsa quas repellendus enim reiciendis quod sequi, veniam, similique praesentium. Iste vero architecto reprehenderit, nulla veniam mollitia libero.</p>
          <br>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vel asperiores quo iusto ipsa quas repellendus enim reiciendis quod sequi, veniam, similique praesentium. Iste vero architecto reprehenderit, nulla veniam mollitia libero.</p>
        </section>
      </main>
    </section>
    <div class="banner">
      <h3>Our Mission</h3>
      <p>
        The motorcycles brought us here, the mountains got us excited, and the people we met along the way kept us coming back. We have combined our passion and know-how to give people the most authentic and unique experiences, in the most beautiful and remote places. We are Open Road Tours.
      </p>
      <nuxt-link class="button-link button-link--tertiary" to="/tours"><span>Contact Us About a Tour</span></nuxt-link>
    </div>
  </main>
</template>

<script>
  import AboutPageHeroContent from '@/components/AboutPageHeroContent'
  import DetailsTable from '@/components/DetailsTable'
  import Article from '@/components/Article'

  export default {
    components: {
      AboutPageHeroContent,
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


