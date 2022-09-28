<script setup>
    import {ref} from "vue"
    const loggedIn = ref(false)
</script>

<template>
    <button :class="loggedIn ? 'bgBlue' : 'bgGreen'" @click="loggedIn = !loggedIn">Press here to {{!loggedIn ? "Log In" : "Log Out"}}!</button>
    <div v-if="loggedIn">This is with if statements: LoggedOut</div>
    <div v-else>This is with if statements: LoggedIn</div>
</template>

<style>
    .bgGreen{
        background-color: green;
    }
    .bgBlue{
        background-color: blue;
    }
</style>