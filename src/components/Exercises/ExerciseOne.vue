<template>
  <div>
    <h1>My First component with title {{ title}}</h1>
    
  </div>
</template>

<script>
export default {

    data(){
        return {
            title: 'This is solomon title page',
            isUpperCase: false,
        }
    }

   

}
</script>

<style scoped>

h1 {
    color: green;
    text-align: center;
    font-weight: bold;
    text-align: center;

   
}

</style>