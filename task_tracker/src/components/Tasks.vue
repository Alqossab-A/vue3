<template>
    <div v-for="task in tasks">
        <h3>{{ task.text }}</h3>
    </div>
</template>

<script lang="ts">
import { PropType } from 'vue';

interface Task {
    id:number;
    text: string;
    day: string;
    reminder: boolean;
}

    export default {
        name: 'Tasks',
        props: {
            tasks: Array as PropType<Task[]>,
        },
    };
</script>