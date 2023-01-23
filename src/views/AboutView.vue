<script setup>
import {useFlash} from "../composables/useFlash";

let {flash} = useFlash();
</script>
<template>
  <div >
    <button @click="flash('Yay','It works on about page','info')">Click me</button>
  </div>
</template>

