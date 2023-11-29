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
    <section>
        <h2>{{ titolo }}</h2>
        <div id="cardsWrapper">
            <AppComicsCard v-for="prodotto in products" :product="prodotto" />
        </div>
    </section>
</template>

<style scoped></style>