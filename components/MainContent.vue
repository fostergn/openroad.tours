<template>
  <section>
    <article>
      <h3>Explore North Vietnam</h3>
      <p>From majestic mountains to deep caves, gushing waterfalls to tranquil lakes, open highways to single-track trails, northern Vietnam has it all. Our 8-day tour allows you to have the adventure of your dreams. We customize a journey for you and your crew based on experience and what you’re looking to get out of your trip, whether it be scenic drives through the mountains or hard climbs up them.</p>
      <div class="cta__wrapper">
        <nuxt-link class="button-link" to="/tours"><span>8 Day Tour</span></nuxt-link>
        <nuxt-link class="button-link button-link--secondary" to="/tours/north-vietnam"><span>Explore</span></nuxt-link>
      </div>
    </article>
    <div class="image__container">
      <img
        src="https://scontent.fmex6-1.fna.fbcdn.net/v/t1.0-9/31224827_1818577911557808_2468753450918215680_o.jpg?_nc_cat=0&oh=8d1be3f1c6ac81225cb2582470284d45&oe=5B84A102"
        class="image">
    </div>
  </section>
</template>

<style lang="scss" scoped>
  section {
    display:flex;
    margin: 0 2rem 8rem;
  }

  article {
    flex: 5;
    margin-right:3rem;
    display:inline-flex;
    flex-direction:column;
  }

  .image__container {
    flex:3;

    & img {
      width:100%;
    }
  }

  h3 {
    margin-bottom:1rem;
    font-size:2.1rem;
    line-height:3rem;
    font-family: 'Playfair Display', serif;
  }

  .cta__wrapper {
    text-align: center;
    margin-top:auto;
    padding-top:1rem;

    & > a {
      margin: 0 1rem;
    }
  }

  .button-link {
    align-self:center;
  }
</style>
