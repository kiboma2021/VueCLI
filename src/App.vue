<template>
  <h1>{{title}}</h1>

  <Modal :header="header" :text="text" theme="sale" />

</template>

<script>
import Modal from './components/Modal.vue'

export default {
  name: 'App',
  components: {Modal},
  data () {
    return {
    title:'My first vue Application :)',
    header: 'Month of Gifts!!!',
    text: 'Nextus is the best tech company'
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

h1 {
  color: red;
  font-style: normal;
}
</style>
