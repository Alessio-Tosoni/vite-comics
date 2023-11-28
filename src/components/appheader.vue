<script>
    export default {
        name: "Appheader",
        data() {
            return {
                paginaAttiva: 0,
                menuLinks: [
                    "CHARACTERS", "COMICS", "MOVIES", "TV", "GAMES", "COLLECTIBLES", "VIDEOS", "FANS", "NEWS", "SHOP"
                ]
            }
        },
        methods:{
            cambiaPagina(index){
                this.paginaAttiva = index
             
            }
        },
        mounted() {
            console.log("Componente AppHeader caricato");
        }
    }
</script>

<template>
    <header class="flex jc-cen ai-cen">
        <div class="flex jc-cen w30 my-8">
            <img class="obj-ft" src="../assets/img/dc-logo.png" alt="">
        </div>
        <div class="flex jc-sb ai-cen w50">
            <p  class="prova mo-8" v-for="(link,index) in menuLinks" v-bind:class="{'paginaAttiva':(index == paginaAttiva)}" @click="cambiaPagina (index)">{{ link }}</p>
        </div>
        
    
    </header>
</template>

<style scoped>
    
</style>