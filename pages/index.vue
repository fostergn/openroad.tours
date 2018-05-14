<template>
  <div>
    <div>
      <div class="video__wrapper">
        <div class="video__offset">
          <div class="video__gradient"></div>
          <HeroContent />
          <no-ssr>
            <plyr-youtube
              id="iIe87ubHQyA"
              allowtransparency
              allow="autoplay"
              loop
              :options="videoOptions"
              :pe="false"
              :crossorigin="true"
            />
          </no-ssr>
        </div>
      </div>
    </div>
    <MainContent/>
    <SecondaryContent/>
  </div>
</template>

<script>
  import HeroContent from '@/components/HeroContent'
  import MainContent from '@/components/MainContent'
  import SecondaryContent from '@/components/SecondaryContent'

  export default {
    computed: {
      videoOptions () {
        return {
          "autoplay": true,
          "loop": { active: true},
          "settings": ['loop'],
          "hideControls": true,
          "muted": true,
          "controls": [],
          "poster": "https://scontent.fmex7-1.fna.fbcdn.net/v/t1.0-9/26239667_1684505514965049_4115751240757307826_n.jpg?_nc_cat=0&oh=3c1c10a997bda10faf3322c2dac68dcf&oe=5B9B1D27"
        }
      }
    },
    components: {
      HeroContent,
      MainContent,
      SecondaryContent
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
