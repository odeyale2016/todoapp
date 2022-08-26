<template>
  <div class="alltasks">
    <h1>All Tasks</h1>
    <div v-for="(task,index) in tasks"  :key="index">
        <ul>
            <li>{{ task.name }} </li><li>{{ task.status }}</li> 
        </ul>

    </div>
    
  </div>
</template>

<script>
export default {
  name: 'AllTasks',
  
  props: ['tasks'],
  data(){
    return {

    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
 display: inline-block;
    list-style-type: none;
    margin: 1%;
    padding: 10px;
    border: 1px;
    border-radius: 5px;
    border-color: brown;
    color:white;
    background-color:cornflowerblue;
}
a {
  color: #42b983;
}
</style>
