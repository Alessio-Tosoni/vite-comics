<script>
    export default {
        name: "store",
        data() {
            return {
                
               storeCat: [{
                src:"../src/assets/img/buy-comics-digital-comics.png",
                type:"DIGITAL COMICS"
               },{
                src:"../src/assets/img/buy-comics-merchandise.png",
                type:"DC MERCHANDISE"
               },{
                src:"../src/assets/img/buy-comics-subscriptions.png",
                type:"SUBSCRIPTION"
               },{
                src:"../src/assets/img/buy-comics-shop-locator.png",
                type:"COMIC SHOP LOCATOR"
               },{
                src:"../src/assets/img/buy-dc-power-visa.svg",
                type:"DC POWER VISA"
               
               }]
            }    
        },
       
        mounted() {
            console.log("Componente store caricato");
        }
    }
</script>

<template>
    <div class="store flex jc-cen ai-cen bg-bl">
        <div class="flex jc-cen ai-cen c-wht">
            <div class="flex jc-cen ai-cen mo-12" v-for="item in storeCat">
                <img class="locandine"  :src="item.src" alt="">
                <p>{{item.type }}</p>
            </div>
            
        </div>  
        
    </div>
</template>

<style scoped>
    
</style>