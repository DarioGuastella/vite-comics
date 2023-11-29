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
        <div class="currentSeries myBtn">
            <h3>CURRENT SERIES</h3>
        </div>
        <div id="cardsWrapper">
            <AppComicsCard v-for="prodotto in products" :product="prodotto" />
        </div>
        <div class="d-flex justify-content-center">
            <button class="myBtn loadBtn btn">
                <h3 class="loadText">LOAD MORE</h3>
            </button>
        </div>


    </section>
</template>

<style scoped>
#cardsWrapper {
    display: flex;
    padding: 2rem;
    flex-wrap: wrap;
}

.myBtn {
    background-color: #0282f9;
    display: inline-block;
    border-radius: 0;
}

.loadText {
    font-size: 0.8rem;
    font-weight: 600;
}

.currentSeries {
    padding: 0.4rem 1.6rem;
    transform: translate(0, -50%);
}

.loadBtn {
    margin-bottom: 1rem;
    padding: 0.6rem 4rem;

}

h3 {
    margin-bottom: 0;
}
</style>