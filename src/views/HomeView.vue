<script setup>
import TheWelcome from "../components/TheWelcome.vue";

// eslint-disable-next-line no-unused-vars
let message = $ref("halo");

let doSomething = () =>{
  alert('doing sth');
}
setTimeout(()=>{
  message = 'I have been changed';
},2000)

</script>

<template>
  <main>
    <TheWelcome />
    <p>{{message}}</p>
    <p><input type="text" v-model="message"></p>
    <button @click="doSomething">Click me</button>
  </main>
</template>
