<template>
  <h1>Exercise Eleven</h1>
  <div>{{ totalItems }} {{ totalCost }}</div>
<ul>
    <li v-for="n in 5" :key="n">
        <a href="#" @click="addToCard(n)">
        Add {{ n }}</a>

    </li>
</ul>
</template>

<script>
export default {
    data(){
        return {
            totalItems:0,
            totalCost:0,
        }


    },

    methods: {
        addToCard(n){
            this.totalItems=this.totalItems+1
            this.totalCost=this.totalCost+n

        },
        formatCurrency(val){
            return '$${val.tofixed(2)}'
        },


    },

}

</script>

<style>

</style>