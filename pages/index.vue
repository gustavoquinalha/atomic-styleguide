<template>
  <div>
  <colors></colors>
  <spaces></spaces>
  <typography></typography>
  </div>
</template>

<script>
  import colors from '@/components/colors';
  import typography from '@/components/typography';
  import spaces from '@/components/spaces';

  export default {
    components: {
      typography,
      colors,
      spaces
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
