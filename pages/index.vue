<template>
  <div>
    <div>
      <div class="video__wrapper">
        <div class="video__offset">
          <div class="video__gradient"></div>
          <HeroContent />
          <HeroVideo />
        </div>
      </div>
    </div>
    <MainContent/>
    <SecondaryContent/>
    <TertiaryContent/>
  </div>
</template>

<script>
  import HeroContent from '@/components/HeroContent'
  import HeroVideo from '@/components/HeroVideo'
  import MainContent from '@/components/MainContent'
  import SecondaryContent from '@/components/SecondaryContent'
  import TertiaryContent from '@/components/TertiaryContent'

  export default {
    components: {
      HeroContent,
      HeroVideo,
      MainContent,
      SecondaryContent,
      TertiaryContent
    }
  }
</script>

<style lang="scss" scoped>

img {
  width:300px;
  height:300px;
}

.plyr--video {
    border-bottom: 4px solid white;
  }

.video__wrapper {
  clip-path: polygon(0 2%, 100% 0%, 100% 96%, 0 100%);
  position:relative;
  overflow:hidden;
  height: calc((9/16) * 100vw);
  transition:.3s;
}

.video__offset {
  position:relative;
  top:-8vw;
  transition:.3s;
  height:100%;

  &:before {
    content: '';
    background-color: #606266;
    background-size:cover;
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    background-image:url('https://scontent.fmex6-1.fna.fbcdn.net/v/t1.0-9/26196171_1681996965215904_1718448388478153231_n.jpg?_nc_cat=0&oh=6b934853211937ae8b7d15c486cfb4ca&oe=5B81AC70')
  }

  &:after {
    content:'';
    width:100%;
    bottom:-2px;
    position:absolute;
    height:8vw;
    background-color: #fff;
    z-index:10;
    clip-path: polygon(0% 0%, 100% 13%, 100% 100%, 0 100%);
  }
}

.video__gradient {
  height: 100%;
  width: 100%;
  z-index: 10;
  position: absolute;
  // background: linear-gradient(to right, rgba(255,0,0,0), rgba(255,255,255,1));
}

section {
  top: -8vw;
  position:relative;
  z-index:10;
}
</style>
