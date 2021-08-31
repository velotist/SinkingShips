<template>
    <div>
        <div class="ship-container">
            <div class="image-container">
                <img :src="imageSource" alt="Ship" />
            </div>
            <div>
                <span>{{ name }}</span>
                <p>{{ size }} Crosses</p>
            </div>
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
