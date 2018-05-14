<template>
  <section>
    <header>
      <h3>Explore Vietnam With Us</h3>
    </header>
    <div class="articles__wrapper">
      <article>
        <div class="image__wrapper">
          <img src="https://scontent.fmex6-1.fna.fbcdn.net/v/t1.0-9/31277625_1818007854948147_8930219885879885824_o.jpg?_nc_cat=0&oh=a2230e2d076f431216b0945f40463432&oe=5B52FCDE" alt="">
        </div>
        <header>
          <h5>Custom Tour</h5>
          <p>Learn more about our tailormade tours that fit any schedule</p>
        </header>
      </article>
      <article>
        <div class="image__wrapper">
          <img src="https://scontent.fmex6-1.fna.fbcdn.net/v/t1.0-9/29541285_1783270695088530_1999488503731287253_n.jpg?_nc_cat=0&oh=fffa78e8d435eeb9fc6290367b6bf649&oe=5B99553A" alt="">
        </div>
        <header>
          <h5>Custom Tour</h5>
          <p>Learn more about our tailormade tours that fit any schedule</p>
        </header>
      </article>
      <article>
        <div class="image__wrapper">
          <img src="https://scontent.fmex6-1.fna.fbcdn.net/v/t1.0-9/29683167_1783270705088529_436138105002130370_n.jpg?_nc_cat=0&oh=ba2de05d3c10b2e94f9a2b2b60077626&oe=5B9925F0" alt="">
        </div>
        <header>
          <h5>Custom Tour</h5>
          <p>Learn more about our tailormade tours that fit any schedule</p>
        </header>
      </article>
    </div>
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
    width:100%;
    padding:4rem 3rem 0;

    & > header {
      margin-bottom:1rem;
    }
  }

  .articles__wrapper {
    display:flex;
  }

  article {

    &:first-child {
      margin-left:0;
    }

    &:last-child {
      margin-right:0;
    }

    margin:1rem;
    box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
    transition: all 0.3s cubic-bezier(.25,.8,.25,1);

    &:hover {
      box-shadow: 0 14px 28px rgba(0,0,0,0.25), 0 10px 10px rgba(0,0,0,0.22);
    }

    &>header {
      padding:1rem;
    }
  }

  h5 {
    font-size: 1.5rem;
    padding: .5rem 0;
  }

  .image {
    &__wrapper {

      & > img {
        width: 100%;
        height: 200px;
        object-fit:cover;
      }
    }
  }
</style>
