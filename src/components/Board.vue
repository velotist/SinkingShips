<template>
    <div style="margin: 50px">
        <h2>{{ boardName }}</h2>
        <table>
            <tr>
                <td class="no-border">1</td>
                <td v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="no-border">2</td>
                <td v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="no-border">3</td>
                <td v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="no-border">4</td>
                <td v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="no-border">5</td>
                <td v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="no-border">6</td>
                <td v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="no-border">7</td>
                <td v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="no-border">8</td>
                <td v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="no-border">9</td>
                <td v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="no-border">10</td>
                <td v-for="n in 10" :key="n"></td>
            </tr>
            <tr>
                <td class="no-border"></td>
                <td class="no-border">A</td>
                <td class="no-border">B</td>
                <td class="no-border">C</td>
                <td class="no-border">D</td>
                <td class="no-border">E</td>
                <td class="no-border">F</td>
                <td class="no-border">G</td>
                <td class="no-border">H</td>
                <td class="no-border">I</td>
                <td class="no-border">J</td>
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
<style>
table,
th,
td {
    border: solid black;
    border-width: 1px;
}
td {
    width: 40px;
    height: 40px;
}
h2 {
    text-align: left;
    margin-left: 10%;
}
.no-border {
    border: 0px;
}
</style>
