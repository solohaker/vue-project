<template>
  <div>
    <h1>Triggering Vue Methods</h1>
    <ul>
        <li v-for="n in 5" :key="n">
            
            <a href="#" @click="triggerAlert(n)">
                <button> Trigger {{ n }}</button> <br><br>
                
                </a>
        </li>
    </ul>

  </div>
</template>

<script>
export default {
    methods: {
        triggerAlert(n){
            alert('that is ${n} has been clicked');
        },
    },

}
</script>
<style scoped>
ul {
    padding-left: 0;
}
li {
    display: block;
    list-style: none;
}
a {
    display: inline-block;
    padding: 10px 20px;
}
</style>

