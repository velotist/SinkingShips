<template>
    <Home />
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Home from './components/Home.vue'

export default defineComponent({
    name: 'App',
    components: {
        Home,
    },
})
</script>

<style>
#app {
    font-family: Papyrus, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
@import './assets/css/board.css';
</style>
