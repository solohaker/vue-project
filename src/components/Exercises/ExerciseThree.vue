<template>
    <div>
        <h1>{{ title }}</h1>
        <h2>{{ subtitle }}</h2>
        <ul>
            <li>{{ items[0] }}</li>
            <li>{{ items[1] }}</li>
            <li>{{ items[2] }}</li>
            <li>{{ items[3] }}</li>
            <li>{{ items[4] }}</li>
            <li>{{ items[5] }}</li>
           
        </ul>
    </div>
  
</template>

<script>
export default {

    data(){
        return {
            title: 'My List component',
            subtitle:'vue JS Basics',
            items: [
                'Item 1',
                'Item 2',
                'Item 3',
                'Item 4',
                'Item 5',
                'Item 6',
            ]
        }
    }
}
</script>


<style>
/* @import '../assets/typography.css'; */
h1{
    font-size: 60px;
}

</style>