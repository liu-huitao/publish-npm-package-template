<template>
  <div id="app">
    <lib-input
      :inputVal="input"
      @changeValue="changeValue"
    ></lib-input>
  </div>
</template>

<script>
import libInput from './lib/index'
export default {
  name: 'app',
  components: {
    libInput
  },
  data () {
    return {
      input: 'xxxx'
    }
  },
  methods: {
    changeValue (val) {
      console.log(val)
    }
  }
}
</script>
