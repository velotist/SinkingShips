<template>
    <div style="display: inline-flex; align-content: center">
        <Board boardName="Ships"></Board>
        <Board boardName="Attack"></Board>
        <div style="margin-left: 20px">
            <Ship name="Flugzeugträger" size="5" imageName="ship5x"></Ship>
            <Ship name="Schlachtschiff" size="4" imageName="ship4x"></Ship>
            <Ship name="U-Boot" size="3" imageName="sub3x"></Ship>
            <Ship name="Zerstörer" size="3" imageName="ship3x"></Ship>
            <Ship name="Patrouillenboot" size="2" imageName="ship2x"></Ship>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Board from '@/components/Board.vue'
import Ship from '@/components/Ship.vue'

export default defineComponent({
    name: 'Home',
    components: {
        Board,
        Ship,
    },
})
</script>
