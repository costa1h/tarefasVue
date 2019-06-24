<template>
    <div class="task-grid">
        <!--<div v-for="task in tasks" :key="task.name">
            {{task.name}}
        </div>-->
        <Task v-for="task in tasks" :key="task.name" :task="task"></task>
    </div>
</template>
<script>
    export default {
        props: {
            tasks: {
                type: Array,
                required: true
            }
        }
    }
</script>