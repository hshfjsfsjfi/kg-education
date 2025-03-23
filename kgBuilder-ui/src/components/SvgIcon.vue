<template>
</template>
<script>
export default {
  name: 'svg-icon',
  props: {
    size: {
      type: [Number, String],
      default: 16
    },
    icon: {
      type: String,
      default: ''
    },
    fill: {
      type: String,
      default: ''
    }
  },
  computed: {
    ClassStyle () {
      return `width:${parseInt(this.size)};height:${parseInt(this.size)};fill:${this.fill};`
    },
    IconName () {
      return `#${this.icon}`
    }
  }
}
</script>

<style scoped>

</style>
