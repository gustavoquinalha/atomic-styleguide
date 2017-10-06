<template>
<div>

  <octocat></octocat>
  <topo></topo>

  <buttons></buttons>
  <typography></typography>
  <colors></colors>
  <grid></grid>
  <spaces></spaces>

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
import buttons from '@/components/buttons';

import rodape from '@/components/rodape';

export default {
  components: {
    topo,
    octocat,
    typography,
    colors,
    spaces,
    grid,
    rodape,
    buttons
  },
  data() {
    return {}
  }
}
</script>

<style lang="scss">
@import './assets/css/main.scss';
</style>
