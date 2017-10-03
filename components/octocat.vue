<template>
<div class="block-oct">
  <div class="oct">
    <a href="https://github.com/gustavoquinalha/styleguide-kit" target="_blank">
      <img src="~/assets/images/octocat.svg" alt="">
    </a>
  </div>
</div>
</template>

<script>
export default {
  name: 'octocat',
  data() {
    return {

    }
  }
}
</script>

<style lang="scss" scoped>
.block-oct {
  position: fixed;
  top: 10px;
  right: 10px;
    .oct {
      transition: .3s;
      img {
        width: 40px
      }
      &:hover {
        transform: scale(1.2, 1.2) rotate(10deg);
      }
    }
}
@media screen and (max-width: 480px) {
  .block-oct {
      .oct {
        img {
          width: 30px
        }
      }
  }
}
</style>
