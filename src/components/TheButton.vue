<template>
    
    <button @click="onClick()"
    
    
    :style="{background:color}" class="btn">{{ text }}</button>
    
</template>
<script>
export default {
    name: 'TheButton',
    props: {
        text: String,
        color: String,

    },
    methods:{
        onclick () {
            // console.log('click');
            this.$emit('toggle-add-task')


        }
    }, 

}





</script>

<style scoped>


</style>