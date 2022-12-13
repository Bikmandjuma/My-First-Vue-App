<template>
  <div id="app">
    <h1>{{title}}-{{names}}</h1>
    <input type="text" ref="name">
    <button @click="handleClick">Click me</button>
    <Modal header="Sing up here !" text="creating youtr account here "/>
  </div>
</template>

<script>
import Modal from './components/Modal.vue'

export default {

  name: 'App',

  components : { Modal },

  data() {
    return {
      title: "Testing !",
      names: "Bikman",
    }
  },

  methods: {
    handleClick() {
      console.log(this.$refs.name),
      this.$refs.name.classList.add('active')
      this.$refs.name.focus()
    }
  }

}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1{
  color:red;
  border-bottom:1px solid #ddd;
  display:inline-block;
  padding:10px;
}
</style>
