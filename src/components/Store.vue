<script>
    export default {
        name: "store",
        data() {
            return {
                
               storeCat: [{
                img:"src\assets\img\buy-comics-digital-comics.png",
                type:"DIGITAL COMICS"
               },{
                img:"C:\BOOLEAN\vite-comics\src\assets\img\buy-comics-merchandise.png",
                type:"DC MERCHANDISE"
               },{
                img:"C:\BOOLEAN\vite-comics\src\assets\img\buy-comics-subscriptions.png",
                type:"SUBSCRIPTION"
               },{
                img:"C:\BOOLEAN\vite-comics\src\assets\img\buy-comics-shop-locator.png",
                type:"COMIC SHOP LOCATOR"
               },{
                img:"C:\BOOLEAN\vite-comics\src\assets\img\buy-dc-power-visa.png",
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
        <div v-for="item in storeCat">
            <img :src="item.img" alt="">
            <p>{{item.type }}</p>
        </div>
    </div>
</template>

<style scoped>
    
</style>