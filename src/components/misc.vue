<script>
    export default {
        name: "Misc",
        data() {
            return {
                dcComics: [
                  "Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"  
                ],
                Shop:[
                    "Shop DC", "Shop DC  Collectibles"
                ],
                DC:[
                    "Terms Of Use", "Privacy policy (new)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops",
                    "CPSC certificates", "Ratings", "Shop Help", "Contact Us"
                ],
               Sites:[
                "DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"

               ]
               
               
            }    
        },
       
        mounted() {
            console.log("Componente misc caricato");
        }
    }
</script>

<template>
    <div class="misc flex jc-sa ai-cen">
        <div class="colSx flex ai-fs  c-wht ml-50">
            <div class=" flex clmn ">
               <div class="flex clmn ">
                    <h1>DC COMICS</h1>
                    <p class="c-gry py-4" v-for="voce in dcComics">{{ voce }}</p>
               </div>
               <div class="flex clmn mt-16">
                    <h1>SHOP</h1>
                    <p class="c-gry py-4" v-for="voce in Shop">{{ voce }}</p>
               </div>
            </div>

            <div class=" flex clmn mo-50">
               <div class="flex clmn ">
                    <h1>DC</h1>
                    <p class="c-gry py-4" v-for="voce in DC">{{ voce }}</p>
               </div>
            </div>

            <div  class=" flex clmn mo-50">
                <div class="flex clmn ">
                    <h1>SITES</h1>
                    <p class="c-gry py-4" v-for="voce in Sites">{{ voce }}</p>
               </div>
            </div>
        </div>
        <div class="colDx mr-50">
            <img class="w70" src="../assets/img/dc-logo-bg.png" alt="">
        </div>
    </div>
        
        
    
</template>