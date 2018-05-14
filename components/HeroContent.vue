<template>
  <div class="video__content">
    <h2>Lorem ipsum dolor sit amet</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Explicabo qui pariatur veniam tenetur voluptates, fugit excepturi soluta ipsa expedita nemo quisquam adipisci mollitia ducimus. Molestias, earum placeat saepe tenetur. Temporibus.</p>
    <nuxt-link class="button-link" to="/tours"><span>Check Out a Tour</span></nuxt-link>
  </div>
</template>

<style lang="scss" scoped>

  .video__content {
    position: absolute;
    top: 50%;
    z-index: 20;
    left: 70%;
    transform: translate(-50%,-50%);
    width: 40%;
    background-color: rgba(255,255,255, .92);
    font-size: 22px;
    padding:.8rem;
    display:flex;
    flex-direction:column;
  }

  h2 {
    margin-bottom:1rem;
    font-size:2.5rem;
    line-height:3rem;
    font-family: 'Playfair Display', serif;
  }

  .button-link {
    margin-top:1rem;
    align-self:center;
  }
</style>
