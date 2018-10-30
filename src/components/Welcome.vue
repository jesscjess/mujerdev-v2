<template>
  <div class="c-panel row no-margin">
    <div class="col-lg-8 col-md-12 c-welcome--image no-padding h-full-screen-height">
      <!-- <img src="@/assets/welcome.png"> -->
    </div>
    <div class="col-lg-4 col-md-12 c-welcome--video no-padding ">
      <div class="container">
        <div class="insta">
          <blockquote class="instagram-media" data-instgrm-permalink="https://www.instagram.com/p/Bn0USAVBv8f/?utm_source=ig_embed&amp;utm_medium=loading" data-instgrm-version="12" style=" background:#FFF; border:0; border-radius:3px; box-shadow:0 0 1px 0 rgba(0,0,0,0.5),0 1px 10px 0 rgba(0,0,0,0.15); margin: 1px; max-width:540px; min-width:326px; padding:0; width:99.375%; width:-webkit-calc(100% - 2px); width:calc(100% - 2px);">
            </blockquote>
        </div>
        <!-- hide on hover or, remove if videoSpritePlayButton opacity = 1 -->
        <div class="play"  @mouseover="playVideo" v-bind:class="{ hide: hidePlay }">
          <font-awesome-icon icon="play" size="10x" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Welcome',
  data () {
    return {
       hidePlay: false
    }
  },
  methods: {
    playVideo: function () {
      this.hidePlay = true;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import '../assets/_variables.scss';
  .c-welcome--image{
    width: 100%;
    background-image: url('../assets/welcome.png');
    background-repeat:no-repeat;
    background-position: center center;
    background-size: cover;

  }
  .c-welcome--video{
    width: 100%;
    min-height: 620px;
    background-color: $coral;

    video{
      width: 100%;
    }
    .container{
      position: relative;
      height: 100%;
    }
    .play{
      background-color: $coral;
      color: #FFFFFF;
      display: flex;
      height: 100%;
      justify-content: center;
      align-items: center;
      cursor: pointer;
      position: absolute;
      top: 0;
      bottom: 0;
      left: 0;
      right: 0;

      &.hide{
        display: none;
      }
    }

    .insta{
      height: 100%;
      display: flex;
      align-items: center;

      .instagram-media{
        border: none !important;
        max-width: 90% !important;
      }
    }

  }
</style>
