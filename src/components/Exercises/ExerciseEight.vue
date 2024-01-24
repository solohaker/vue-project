<template>
  <div>

    <h1>Looping via Arrays</h1>
    <ul>
        <li 
        v-for="(item,n) in interests" :key="n">
        {{ item }}

        </li>
    </ul>


  </div>
</template>

<script>
export default {
    data(){
        return {
            interests: ['TV','Games','Sports'],

        }
    },

}
</script>

<style>

</style>