<template>
    <div>
        <h1 :class="$style.title">{{ title }}</h1>
        <h2 :class="$style.subtitle"> {{  subtitle }}</h2>
    </div>
  
</template>

<script>
export default {
    data(){
        return {
            title: 'CSS module component!',
            subtitle: 'The fourth Exercise',
        }
    },

}
</script>

<style module>
h1,
h2 {
    text-align: center;
}
.title {
    color: lightcoral;
}

.subtitle {
    color: blueviolet;
    font-style: italic;

}

</style>