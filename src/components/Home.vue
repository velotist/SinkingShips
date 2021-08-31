<template>
    <div class="home-container">
        <Board boardName="Ships"></Board>
        <Board boardName="Attack"></Board>
        <div class="home-ship-container">
            <Ship name="Aircraft carrier" size="5" imageName="ship5x"></Ship>
            <Ship name="Battleship" size="4" imageName="ship4x"></Ship>
            <Ship name="Submarine" size="3" imageName="sub3x"></Ship>
            <Ship name="Destroyer" size="3" imageName="ship3x"></Ship>
            <Ship name="Patrol Boat" size="2" imageName="ship2x"></Ship>
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
