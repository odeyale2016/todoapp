<template>
  <img alt="Vue logo" src="./assets/alphatech.png">
  <NavBar></NavBar>
  <HelloWorld msg="Welcome to Alphatech Solutions Todo-App with vuejs"/>
  {{ content }}
  <AllTasks :tasks="tasks"></AllTasks>
  <CompletedTasks :tasks="tasks"></CompletedTasks>
  <PendingTasks :tasks="tasks"></PendingTasks>

</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import NavBar from './components/NavBar.vue'
import AllTasks from './components/AllTasks.vue'
import CompletedTasks from './components/CompletedTasks.vue'
import PendingTasks from './components/PendingTasks.vue'



export default {
  name: 'App',
  data(){
    return {
    content: 'This is my first site developed with vue js',
    tasks: [
      {name: 'Creation of wireframes for all the pages of the website', status:'Completed'},
      {name: 'Building of the Homepage of the website', status:'Completed'},
      {name: 'Backend development tasks', status:'Pending'},
      {name: 'Linking of Backend and Frontend together', status:'Pending'}
    ]
    }
  },
  components: {
    HelloWorld,
    NavBar,
    AllTasks,
    CompletedTasks,
    PendingTasks
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
