<script setup>
import {ref, onMounted} from "vue"
    let string = ref("")
    function templateString(){
        string = "--- This is my string :) ---"
    }
    templateString()
</script>

<template>
  <div>
    This is my navBar component :)
    <p> And this is what my sum is printing: {{2+2}}</p>
    <p> And this is what my function returns {{string}}</p>
  </div>
</template>

<style>
    button{
        
    }
</style>