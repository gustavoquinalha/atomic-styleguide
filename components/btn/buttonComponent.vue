<template>
<div>
  <div class="" v-if="size === 'small'">
    <button type="button" name="button" class="btn btn-small" :class="[type]" :style="{ background: color, color: fontColor, borderRadius: borderRadius }">{{value}}</button>
  </div>

  <div class="" v-if="size === 'medium'">
    <button type="button" name="button" class="btn" :class="[type]" :style="{ background: color, color: fontColor, borderRadius: borderRadius }">{{value}}</button>
  </div>

  <div class="" v-if="size === 'large'">
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
      default: 'medium',
		},
		type: {
			type: String,
      default: 'default',
		},
		color: {
			type: String,
      default: '#ddd',
		},
		fontColor: {
			type: String,
      default: '#333',
		},
		borderRadius: {
			type: String,
      default: '4px',
		},
		width: {
			type: String,
		}
	}
}
</script>

<style lang="scss" scoped>

</style>
