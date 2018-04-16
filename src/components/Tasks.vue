<template>
    <div class="tasksWrapper">
        <div class="tasks">
            <template v-if="tasks.length">
                <Task v-for="task in tasks" :key="task.id" :task="task"></Task>
            </template>
            <span v-else>No tasks</span>
        </div>
        <hr>
        <form action="">
            Form
        </form>
    </div>
</template>

<script>
    import Task from './Task'
    export default {
        components: {
            Task
        },
        name: "Tasks",
        data() {
            return {
                tasks: [
                    { id: 1, body: 'Task one', done: false },
                    { id: 2, body: 'Task two', done: false },
                    { id: 3, body: 'Task three', done: false }
                ]
            }
        }
    }
</script>

<style scoped>

</style>