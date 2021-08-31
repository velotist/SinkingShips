<template>
    <div class="board-container">
        <h2>{{ boardName }}</h2>
        <table>
            <tr>
                <td class="board-table_no-border">1</td>
                <td class="board-table_td" v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="board-table_no-border">2</td>
                <td class="board-table_td" v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="board-table_no-border">3</td>
                <td class="board-table_td" v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="board-table_no-border">4</td>
                <td class="board-table_td" v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="board-table_no-border">5</td>
                <td class="board-table_td" v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="board-table_no-border">6</td>
                <td class="board-table_td" v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="board-table_no-border">7</td>
                <td class="board-table_td" v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="board-table_no-border">8</td>
                <td class="board-table_td" v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="board-table_no-border">9</td>
                <td class="board-table_td" v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="board-table_no-border">10</td>
                <td class="board-table_td" v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="board-table_no-border"></td>
                <td class="board-table_no-border">A</td>
                <td class="board-table_no-border">B</td>
                <td class="board-table_no-border">C</td>
                <td class="board-table_no-border">D</td>
                <td class="board-table_no-border">E</td>
                <td class="board-table_no-border">F</td>
                <td class="board-table_no-border">G</td>
                <td class="board-table_no-border">H</td>
                <td class="board-table_no-border">I</td>
                <td class="board-table_no-border">J</td>
            </tr>
        </table>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    name: 'Board',
    props: {
        boardName: String,
        required: {
            type: Boolean,
            default: true,
        },
    },
})
</script>
