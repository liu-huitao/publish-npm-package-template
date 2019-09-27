<template>
  <div id="app">
    姓名：<input
      v-model="inputValue"
      type="text"
      @change="changeValue"
    >
  </div>
</template>

<script>
export default {
  name: 'libInput',
  props: {
    inputVal: {
      type: String,
      default: ''
    }
  },
  data () {
    return {
      inputValue: this.inputVal
    }
  },
  methods: {
    changeValue () {
      this.$emit('changeValue', this.inputValue);
    }
  }
}
</script>
