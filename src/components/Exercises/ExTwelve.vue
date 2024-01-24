<template>
  <h1>Excercise Twelve</h1>
 <ul>

    <li v-for="(i,n) in list" :key="n">
{{ i }}
<a @click="deleteItem(i)">Delete</a>
    </li>
 </ul>




</template>

<script>
export default {
    data(){
        return {
            list: [
                'Apex legends',
                'a plauge tale: innocence',
                'Art sqool',
            ],
        }
    },
   /*  beforeCreate(){
        alert('beforeCreate: data is static, that it')
    },
    created(){
        alert('created: data and events ready,but no DOM')
    },
    mounted(){
        alert('mounted: DOM ready to use')
    }, */
    methods: {
        deleteItem(value){
            this.list=this.list.filter(i=>i!==value)
        },
    }



}
</script>

<style>

</style>