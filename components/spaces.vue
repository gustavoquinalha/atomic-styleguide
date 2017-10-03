<template>
<div class="size margin">

  <div class="example">
    <titleComponent>
       <span slot="title">Spaces</span>
    </titleComponent>
    <div class="container wrap padding-top-20 border-box padding-20">
      <div class="flex-basis-300 flex-grow-1 container column container-space">
        <strong>Margin (left, right, top, bottom)</strong>
        <div class="bspace">
          without margin
        </div>

        <div class="bspace margin-left-10">
          margin-left-10
        </div>

        <div class="bspace margin-left-20">
          margin-left-20
        </div>

        <div class="bspace margin-left-30">
          margin-left-30
        </div>

        <div class="bspace margin-left-40">
          margin-left-40
        </div>

        <div class="bspace margin-left-50">
          margin-left-50
        </div>
      </div>

      <div class="flex-basis-300 flex-grow-1 container column container-space">
        <strong>Padding (left, right, top, bottom)</strong>
        <div class="bspace">
          without padding
        </div>

        <div class="bspace padding-left-10">
          padding-left-50
        </div>

        <div class="bspace padding-left-20">
          padding-left-50
        </div>

        <div class="bspace padding-left-30">
          padding-left-50
        </div>

        <div class="bspace padding-left-40">
          padding-left-50
        </div>

        <div class="bspace padding-left-50">
          padding-left-50
        </div>
      </div>
    </div>

    <div class="container wrap border-box margin-20 container-space">
      <div class="bspace space">
        <strong>width 90% margin 0 auto</strong>
      </div>
    </div>

  </div>

</div>
</template>

<script>
import titleComponent from '@/components/titleComponent'

export default {
  components: {
    titleComponent
  },
  name: 'spaces',
  data() {
    return {}
  }
}
</script>

<style lang="scss" scoped>
.container-space {
    // border-left: 5px solid #000;
    margin-bottom: 20px;
    .bspace {
        margin-bottom: 5px;
        border-left: 2px solid #50fa7b;
        font-size: 14px;
        padding-top: 10px;
        padding-bottom: 10px;
    }
    .bspace.space {
        border-right: 2px solid #50fa7b;
    }
}
</style>
