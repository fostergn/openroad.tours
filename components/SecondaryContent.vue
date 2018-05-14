<template>
  <section>
    <header>
      <h3>Get In Touch With Us</h3>
    </header>
    <article>
      <div class="form__context">
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Saepe, eligendi? Ipsa reprehenderit ex quo eos officiis. Itaque id, sequi soluta atque, facilis, dignissimos doloribus iure ex totam quia officia, saepe. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Saepe, eligendi? Ipsa reprehenderit ex quo eos officiis. Itaque id, sequi soluta atque, facilis, dignissimos doloribus iure ex totam quia officia, saepe.</p>
        <div class="cta__wrapper">
          <nuxt-link class="button-link button-link--tertiary" to="/tours"><span>Contact Us About a Tour</span></nuxt-link>
        </div>
      </div>
      <div class="form__container">
        <Form />
      </div>
    </article>
  </section>
</template>

<script>
  import Form from '@/components/GeneralForm'

  export default {
    components: {
      Form
    }
  }
</script>

<style lang="scss" scoped>
  section {
    background-color:#3f46ad;
    color:#fff;
    width:100%;
    padding:1rem 3rem 3rem;
  }

  article {
    display:flex;
  }

  .form__context {
    flex:2;
  }

  .form__container {
    flex:5;
  }

  h3 {
    margin-bottom:1rem;
    margin-top:2rem;
    text-align:center;
    color:#fff;
    margin-bottom:2rem;
  }

  p {
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
