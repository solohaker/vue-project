<template>
    
    <header>
        <!-- <h1>Task Tracker</h1> -->
        <h1>{{title}}</h1>
        <TheButton @toggle-add-task="$emit('toggle-add-task')" text="Add Task" color="green"/>
        <!-- <TheButton text="Update Task" color="yellow"/>
        <TheButton text="Add Task" color="lightblue"/>
        <TheButton text="Delete Task" color="red"/> -->


    </header>
</template>

<script>
import TheButton from './TheButton.vue'







export default {
    name: 'TheHeader',
    // props: ['title'],
    props: { 
        title: String,
      
       
    },
    components: {
        TheButton

    }

}


</script>

<style scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
    margin-top: 10px;
    border: 1px solid black;

}



</style>