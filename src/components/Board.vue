<template>
    <div class="board-container_margin">
        <h2>{{ boardName }}</h2>
        <table>
            <tr v-for="number in 10" :key="number">
                <td class="board-table_td-number">
                    {{ number }}
                </td>
                <td
                    v-for="n in letters.length"
                    :key="n"
                    v-bind:id="`${letters[n - 1]}.${number}`"
                    class="board-table_td"
                ></td>
            </tr>
            <tr>
                <td class="board-table_no-border"></td>
                <td
                    class="board-table_no-border"
                    v-for="letter in letters"
                    :key="letter"
                >
                    {{ letter }}
                </td>
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
    data() {
        return {
            letters: ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J'],
        }
    },
})
</script>
