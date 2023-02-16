<template>
  <h2>{{title}}</h2>
  <input type="text" ref="name">
  <button @click="className">Click me</button>

</template>

<script>

export default {
  name: 'App',
  data () {
    return {
    title:'My first vue Application :)'
    }
  },
  methods: {
    className() {
      this.$refs.name.classList="active"
      this.$refs.name.focus()
    }
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
