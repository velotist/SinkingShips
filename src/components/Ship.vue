<template>
    <div>
        <div style="margin: 10px; display: inline-flex">
            <img :src="imageSource" alt="Ship" />
        </div>
        <div>
            <p>{{ name }}</p>
            <p>{{ size }} Kreuze</p>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    name: 'Ship',
    props: {
        name: String,
        size: String,
        imageName: String,
    },
    computed: {
        imageSource() {
            return require(`../assets/images/${this.imageName}.png`)
        },
    },
})
</script>
