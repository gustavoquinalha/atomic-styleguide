<template>
<div class="size margin">

  <div class="example">
    <div class="title padding-left-20 color-primary">
      <h3>Grid</h3>
    </div>
    <div class="container">
      <div class="box-grid" v-for="(x, index) in 12">
        {{index + 1}}
      </div>
    </div>

  </div>
</div>
</template>

<script>
export default {
  name: 'grid',
  data() {
    return {}
  }
}
</script>

<style lang="scss" scoped>
.box-grid {
  background: #e2e2e2;
  margin: 5px;
  min-height: 300px;
  flex-grow: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
