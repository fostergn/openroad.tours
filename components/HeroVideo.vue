<template>
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
</template>

<script>
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
  }
</script>
