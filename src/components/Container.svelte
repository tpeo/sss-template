<script>
  export let typography = false;
</script>

<style lang="scss">
  @import "./GlobalStyle/theme.scss";
  div {
    width: 90%;
    box-sizing: border-box;
    max-width: 62em;
    margin: auto;
    position: relative;
    @include breakpoint("l") {
      max-width: 80em;
    }
    @include breakpoint("xl") {
      max-width: 90em;
    }
    &.typography {
      @extend .typography;
    }
  }
</style>

<div class:typography>
  <slot />
</div>
