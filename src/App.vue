<template>
  <CodingInstructions title="Coding challenge"/>
</template>

<script>
import CodingInstructions from './components/CodingInstructions.vue'

export default {
  name: 'App',
  components: {
    CodingInstructions
  }
}
</script>

<style lang="less">
  @import './assets/variables.less';

  body {
    font-family: @font-family;
    background-color: @app-background-color;
    color: @default-color;
    margin: 1.5rem;
  }
</style>
