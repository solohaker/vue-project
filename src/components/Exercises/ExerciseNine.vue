<template>
  <div>
    <h1>Looping Through an Array of Objects</h1>
    <ul>
        <li v-for="(item,n) in interests" :key="n">
            {{ item }}
            <ol>
                <li v-for="(fav,m) in title " :key='m'>
{{ title }}
                </li>
            </ol>
        </li>
    </ul>

  </div>
</template>

<script>
export default {
    data(){
        return{
            title: ['TV','Sports','Game'],
            interests: ['A','B','C'],

        }
    }

}
</script>

<style>

</style>