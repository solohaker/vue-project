<template>
    <selection>
  <div class="form">
    <label for="">
        <input type="text" v-model="name">
    </label>
    <label for="">
        Preferd JavaScript style
        <select name="language" v-model="language">
        <option value="JS">JS</option>
        <option value="TypeScript">TypeScript</option>
        <option value="CoffeeScript">CoffeeScript</option>
        <option value="Dart">Dart</option>
        
        </select>

    </label>
    
    
</div>

<ul class="overview">
  <li><strong>Overview</strong></li>
  <li>Name: {{ name }}</li>
  <li>Preference: {{ language }}</li>


</ul>

</selection>
</template>

<script>
export default {
    data(){
        return {
            name: '',
            language: '',
        }
    },

}
</script>

<style>
.form {
    display: flex;
    justify-content: space-between;
    min-width: 800px;
    padding: 40px 20px;
    border-radius: 10px;
}

.overview {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    max-width: 300px;
    margin: 40px auto;
    padding: 40px 20px;
    border-radius: 10px;
    border: 1px solid #ececec;
  
}
   li {
            margin-top: 20px;
            list-style: none;
        }

</style>