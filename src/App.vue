<script setup>
import TaskItem from './components/TaskItem.vue'

const tasks = [
  {id: 1, title: "посуда", text: "сегодня нужно обязательно помыть посуду!"},
  {id: 2, title: "уроки", text: "нужно сделать все уроки и долги по учебе"},
  {id: 3, title: "собака", text: "нужно обязательно погулять с собакой"},
  {id: 4, title: "купить продукты", text: "молоко, чай, яйца, хлеб"}
]
</script>

<template>
<h1>Мой список дел</h1>
<TaskItem v-for = "task in tasks" :key="task.id" :task="task"/>  
</template>


