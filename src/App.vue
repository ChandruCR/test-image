<template>
  <div id="app">
    <screenshot :key="componentKey"/>
  </div>
</template>

<script>
import Screenshot from "./components/Screenshot.vue"

export default {
  name: "app",
  data: () => ({
    componentKey: 1
  }),
  components: {
    Screenshot
  },
  mounted: function() {
    let vm = this 
    setInterval(() => {
      vm.componentKey++
    }, 10000)
  }
}
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
