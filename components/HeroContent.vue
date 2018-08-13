<template>
  <div class="video__content">
    <h2>We are Open Road Tours</h2>
    <p>The motorcycles brought us here, the mountains got us excited, and the people we met along the way kept us coming back.</p>
    <p>We have combined our passion and know-how to give people the most authentic and unique experiences, in the most beautiful and remote places.</p>
    <nuxt-link class="button-link" to="/tours"><span>Check Out a Tour</span></nuxt-link>
  </div>
</template>

<style lang="scss" scoped>

  .video__content {
    width:500px;
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

  p {
    margin-bottom:.5rem;
  }
</style>
