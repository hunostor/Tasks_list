<template>
    <div class="task">
        {{ task.body }}
    </div>
</template>

<script>
    export default {
        name: "Task",
        props: ['task']
    }
</script>

<style scoped>

</style>