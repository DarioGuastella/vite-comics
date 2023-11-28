<script>
import AppBuySection from "../components/AppBuySection.vue"
export default {
    components: {
        AppBuySection
    },

}
</script>
<template>
    <section>
        <div class="container">
            <h3> --Content goes here-- </h3>
        </div>
    </section>
    <AppBuySection />
</template>
<style scoped>
section {
    background-color: black;
    color: white;
}

div h3 {
    padding: 3rem;
    margin: 0;
}
</style>