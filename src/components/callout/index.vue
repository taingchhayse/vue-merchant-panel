<template>
  <div class="callout-wrapper">
    <span class="callout-icon">{{ boxData.icon }}</span>
    <div>
      <span class="callout-box-text">{{ boxData.text }}</span>
      <slot></slot>
    </div>
  </div>
</template>

<script>
// import pathToRegexp from 'path-to-regexp'

export default {
  name: 'Callout',
  props: {
    boxData: {
      type: Object,
      required: true
    }
  },
  data() {
    return {
    }
  },
  watch: {
  },
  created() {
  },
  methods: {

  }
}
</script>

<style lang="scss" scoped>
.callout-wrapper{
    width: 100px;
    height: 100px;
    background-color: red;
}
</style>
