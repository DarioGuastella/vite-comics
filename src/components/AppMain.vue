<script>
import AppBuySection from "./AppBuySection.vue"
import AppJumbo from "./AppJumbo.vue"
export default {
    components: {
        AppBuySection,
        AppJumbo
    },

}
</script>
<template>
    <section>
        <AppJumbo />
        <div class="container">
            <h3> --Content goes here-- </h3>
        </div>
    </section>
    <AppBuySection />
</template>
<style scoped>
section {
    background-color: #222;
    color: white;
}

div h3 {
    padding: 3rem;
    margin: 0;
}
</style>