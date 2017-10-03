<template>
  <div>
  <octocat></octocat>
  <topo></topo>

  <colors></colors>
  <spaces></spaces>
  <grid></grid>
  <typography></typography>

  <rodape></rodape>
  </div>
</template>

<script>
  import octocat from '@/components/octocat';
  import topo from '@/components/topo';

  import colors from '@/components/colors';
  import typography from '@/components/typography';
  import spaces from '@/components/spaces';
  import grid from '@/components/grid';

  import rodape from '@/components/rodape';

  export default {
    components: {
      topo,
      octocat,
      typography,
      colors,
      spaces,
      grid,
      rodape
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
