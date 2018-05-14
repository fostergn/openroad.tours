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
}

.video__offset {
  position:relative;
  top:-8vw;

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
