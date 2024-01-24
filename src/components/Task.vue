<template>
    <div @dblclick="$emit('toggle-reminder',task.id)"
    :class="[task.reminder?'reminder':
'','task']">
         <h3>{{ task.text }}</h3>
         <i @click="$emit('delete-task',task.id)" class="fas fa-times">icon</i>
         <p>{{ task.day }}</p>


    </div>
   
    

</template>

<script>
export default {
    name: 'Task',

    props: {
        task:Object
    },

/*     methods: {
        onDelete(id) {
            // console.log(id);
            this.$emit('delete-task',id)
        },

    }, */
}



</script>

<style scoped>
.fas {
    color: red;

}
.task h3 {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.task.reminder {
    border-left: 5px solid green;
}

.task {
    background: #f4f4f4;
    margin: 5px;
    padding: 10px 20px;
    cursor: pointer;
}


</style>