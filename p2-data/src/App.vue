<script setup>
import HelloWorld from './components/HelloWorld.vue'
import {data} from './data/data.js'
const welcome = 'Welcome to VueJs and learning!'

function GetDate(){
  const date = new Date();
  return date.toDateString();
}


</script>

<template>
   <div>
        <h1> {{ data.message }} </h1>
        <h2>Today is {{ GetDate() }}</h2>
        <h2>You Have {{ data.task.length }} Task today!</h2>
    </div>

</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
