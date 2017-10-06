<template>
<div>
  <div class="btn-space" v-if="size === 'small'">
    <button type="button" name="button" class="btn btn-small" :class="[type]" :style="{ background: color, color: fontColor, borderRadius: borderRadius, width: width  }">{{value}}</button>
  </div>

  <div class="btn-space" v-if="size === 'medium'">
    <button type="button" name="button" class="btn" :class="[type]" :style="{ background: color, color: fontColor, borderRadius: borderRadius, width: width  }">{{value}}</button>
  </div>

  <div class="btn-space" v-if="size === 'large'">
    <button type="button" name="button" class="btn btn-large" :class="[type]" :style="{ background: color, color: fontColor, borderRadius: borderRadius, width: width }">{{value}}</button>
  </div>

</div>
</template>

<script>
export default {
  name: 'buttonComponent',
  data() {
    return {
    }
  },
  props: {
		value: {
			type: String
		},
		size: {
			type: String,
      default: 'medium'
		},
		type: {
			type: String,
      default: ''
		},
		color: {
			type: String,
      default: ''
		},
		fontColor: {
			type: String,
      default: ''
		},
		borderRadius: {
			type: String,
      default: ''
		},
		width: {
			type: String,
      default: ''
		}
	}
}
</script>

<style lang="scss" scoped>
.btn-space {
  width: 100%;
}
</style>
