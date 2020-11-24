<template>
  <div id="app">
    <Todos v-bind:todos="todos"/>
  </div>
</template>

<script>
import Todos from  "./components/Todos"

export default {
  name: 'App',
  components: {
    Todos
  },
  data(){
    return {
      todos:[
        {
          id: 1, 
          title: "Eat Cheese",
          completed: false
        },
        {
          id: 2,
          title: "Eat Cow",
          completed: false
        },
        {
          id: 3,
          title: "Eat Mango",
          completed: true
        }
      ]
    }
  }
}
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: Arial, Helvetica, sans-serif;
}
</style>
