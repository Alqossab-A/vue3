<script>
    import Button from './Button.vue'

    export default {
        name: 'Header',
        props: {

        },
        components: {
            Button
        }
    };
</script>

<template>
    <header>
        <h1>Task Tracker </h1>
        <Button />
    </header>
</template>

<style scoped>
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;
    }
</style>
