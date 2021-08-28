<template>
    <div>
        <h1>{{ msg }}</h1>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    name: 'Game',
    props: {
        msg: String,
    },
})
</script>
