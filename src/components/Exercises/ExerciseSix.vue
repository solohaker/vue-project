
<template>
    <div>
        <h1 v-if="true" v-once v-text="title"></h1>
    <h2 v-else-if="false" v-html="html"></h2>
    <a 
    v-else
    :href="link.url"
    :target="link.target"
    :tabindex="link.tabindex"
    v-text="link.title"
    >
</a>
    
    </div>
  
  
</template>

<script>
export default {
    data(){
        return {
            title: 'Directive Text',
            html: 'Stylize</br>HTML in<br/><b>your data</b>',
            // name:'solomon'


        }
    },

}
</script>



<style scoped>
h2 {
    margin: 40px 0 0;
    font-weight: normal;
}

</style>

