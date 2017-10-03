<template>
<div class="size margin">

  <div class="example">
    <div class="title padding-left-20 color-primary">
      <h3>Spaces</h3>
    </div>
    <div class="container wrap margin-left-20 padding-top-20">
      <div class="flex-basis-300 flex-grow-1 container column container-space">
        <strong>Margin (left, right, top, bottom)</strong>
        <div class="space">
          without margin
        </div>

        <div class="space margin-left-10">
          margin-left-10
        </div>

        <div class="space margin-left-20">
          margin-left-20
        </div>

        <div class="space margin-left-30">
          margin-left-30
        </div>

        <div class="space margin-left-40">
          margin-left-40
        </div>

        <div class="space margin-left-50">
          margin-left-50
        </div>
      </div>

      <div class="flex-basis-300 flex-grow-1 container column container-space">
        <strong>Padding (left, right, top, bottom)</strong>
        <div class="space">
          without padding
        </div>

        <div class="space padding-left-10">
          padding-left-50
        </div>

        <div class="space padding-left-20">
          padding-left-50
        </div>

        <div class="space padding-left-30">
          padding-left-50
        </div>

        <div class="space padding-left-40">
          padding-left-50
        </div>

        <div class="space padding-left-50">
          padding-left-50
        </div>
      </div>
    </div>

  </div>



</div>
</template>

<script>
export default {
  name: 'spaces',
  data() {
    return {}
  }
}
</script>

<style lang="scss" scoped>
.container-space {
  border-left: 5px solid #000;
  margin-bottom: 20px;
  .space {
    margin-bottom: 5px;
    border-left: 2px solid #50fa7b;
    font-size: 10px;
    padding-top: 10px;
    padding-bottom: 10px;
  }
}
</style>
