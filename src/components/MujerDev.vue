<template>
  <div class="c-panel h-full-screen-height">
    <div class="col-sm-12">
      <a target="_blank" href="https://www.instagram.com/mujerdev/" >@mujerdev</a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MujerDev',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import '../assets/_variables.scss';
  .c-panel{
    background-color: $peach;
    display: flex;
    align-items: center;
    justify-content: center;
    a{  
      color: $light-text;
      font-size: 15vw;
      text-shadow: 9px 7px #000000;
      font-family: 'Pacifico', cursive;

      @include respond-below(sm) {
        text-shadow: 3px 4px #000000;
      }
      &:hover{
        color: $coral;
        text-decoration: none;
      }
    }
  }
</style>
