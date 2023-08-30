<template>
  <canvas id="test"></canvas>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import { fabric } from 'fabric'

@Options({
  components: {
    
  },
})
export default class App extends Vue {
  created (): void {
    console.log('test', new fabric.Canvas('test'))
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
