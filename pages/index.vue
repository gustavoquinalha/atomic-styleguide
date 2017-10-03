<template>
  <div>
  <colors></colors>
  <spaces></spaces>
  <grid></grid>
  <typography></typography>
  </div>
</template>

<script>
  import colors from '@/components/colors';
  import typography from '@/components/typography';
  import spaces from '@/components/spaces';
  import grid from '@/components/grid';

  export default {
    components: {
      typography,
      colors,
      spaces,
      grid
    },
    data() {
      return {
      }
    }
  }
</script>

<style lang="scss">
  @import './assets/css/main.scss';
</style>
