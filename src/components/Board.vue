<template>
    <div class="board-container">
        <h2>{{ boardName }}</h2>
        <table>
            <tr v-for="n in letters.length" :key="n">
                <td class="board-table_no-border">
                    {{ n }}
                </td>
                <td
                    class="board-table_td"
                    v-for="n in letters.length"
                    :key="n"
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
