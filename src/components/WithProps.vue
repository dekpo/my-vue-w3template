<script>
export default{
    props : {
        text : {
            type: String
        }
    },
    methods:{
        loadPage(page){
            this.$parent.loadPage(page);
        }
    }
}
</script>

<template>
<div class="w3-center">
<h2>{{text}}</h2>
<button class="w3-button w3-black" @click="loadPage('contact')">Load Contact !</button>
</div>
</template>