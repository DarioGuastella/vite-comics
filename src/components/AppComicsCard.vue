<script>
export default {
    name: "AppComicsCard",
    props: {
        product: Object
    }
}
</script>
<template>
    <div class="myCard">
        <img :src="product.thumb" alt="">
        <h3>{{ product.series.toUpperCase() }}</h3>
    </div>
</template>
<style scoped>
h3 {
    margin-bottom: 0;
    font-weight: 500;
    font-size: 0.9rem;
    padding: 1rem 0 2rem 0;
    color: #d3cfcf;
}

img {
    height: 12rem;
    width: 12rem;
    object-fit: cover;
    object-position: top;
}

.myCard {
    width: calc(100% / 6);
}
</style>