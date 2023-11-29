<script>
export default {
    name: "AppHeader",
    data() {
        return {

            headerLinks: [
                {
                    text: "CHARACTERS",
                    url: "#",
                },
                {
                    text: "COMICS",
                    url: "#",
                },
                {
                    text: "MOVIES",
                    url: "#",
                },
                {
                    text: "TV",
                    url: "#",
                },
                {
                    text: "GAMES",
                    url: "#",
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                },
                {
                    text: "VIDEOS",
                    url: "#",
                },
                {
                    text: "FANS",
                    url: "#",
                },
                {
                    text: "NEWS",
                    url: "#",
                },
                {
                    text: "SHOP",
                    url: "#",
                },
            ]
        }
    }
}
</script>
<template>
    <header class="d-flex container justify-content-between">
        <!-- Logo -->
        <img class="p-4" src="../assets/img/dc-logo.png" alt="">
        <!-- navigatore -->
        <nav class="d-flex align-items-center">
            <a class="mx-3" v-for="link in headerLinks" :href="link.url">{{ link.text }}</a>
        </nav>
    </header>
</template>
<style scoped>
nav a {
    text-decoration: none;
    color: #555;
    font-weight: 600;
}
</style>