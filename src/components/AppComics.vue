<script>
import AppComicsCard from './AppComicsCard.vue'

export default {
    name: "AppComics",
    props: ["products"],
    components: {
        AppComicsCard
    }
}
</script>

<template>
    <section class="container">
        <div id="cardsWrapper">
            <AppComicsCard v-for="prodotto in products" :product="prodotto" />
        </div>
    </section>
</template>

<style scoped>
#cardsWrapper {
    display: flex;
    padding: 2rem;
    flex-wrap: wrap;
}
</style>