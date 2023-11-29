<script>
    export default {
        name: "AppCard",
        props: ["fumetti"]
       
      
        
    }
</script>

<template>
<div class="card c-wht fs-14">
    <img  :src="fumetti.thumb" alt="">
    <p>{{ fumetti.series }}</p>
</div>

</template>
<style scoped>
    .card{
        width: calc(100% / 6);
        margin: 12px auto;
    }
    img{
        width: 60%;
        height: 70%;
        }
</style>