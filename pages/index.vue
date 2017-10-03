<template>
  <div>
  <colors></colors>
  <typography></typography>
  </div>
</template>

<script>
  import colors from '@/components/colors';
  import typography from '@/components/typography';

  export default {
    components: {
      typography,
      colors
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
