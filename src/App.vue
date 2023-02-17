<template>
  <h1>{{title}}</h1>
  <p>Welcome...</p>
  <button @click="toggleModal">Open Modal</button>

  <div v-if="showModal">
    <Modal :header="header" :text="text" theme="sale" />
  </div>

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
    text: 'Nextus is the best tech company',
    showModal: false,
    }
  },
  methods: {
    className() {
      this.$refs.name.classList="active"
      this.$refs.name.focus()
    },

    toggleModal() {
      this.showModal = !this.showModal
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
