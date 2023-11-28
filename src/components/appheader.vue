<script>
    export default {
        name: "appheader",
        data() {
            return {
                menuLinks: [
                    "CHARACTERS", "COMICS", "MOVIES", "TV", "GAMES", "COLLECTIBLES", "VIDEOS", "FANS", "NEWS", "SHOP"
                ]
            }
        },
        mounted() {
            console.log("Componente AppHeader caricato");
        }
    }
</script>

<template>
    <header>
        <nav>
            <a v-for="link in menuLinks" :href="link.url">{{ link.text }}</a>
        </nav>
    </header>
</template>

<style scoped>
    nav a {
        margin: 0 1rem;
    }
</style>