<script setup lang="ts">
const props = defineProps<{task:{
    title: string;
    text: string;
}}>()
</script>

<template>
    <div class="task-item">
        <h3>{{ props.task.title }}</h3>
        <p>{{ props.task.text }}</p>
    </div>


</template>

<style>
.task-item{
    border: 2px solid #42b983;
    border-radius: 10px;
    padding: 15px;
    margin-bottom: 15px;
    background-color: #f9f9f9;
}
h3 {
    margin-top: 0;
    color: #2c3e50;
}
p{
    color: #2c3e50; 
}
</style>