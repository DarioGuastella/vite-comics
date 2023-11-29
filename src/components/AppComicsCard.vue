<script>
export default {
    name: "AppComicsCard",
    props: {
        product: Object
    }
}
</script>
<template>
    <div class="">
        <img :src="product.thumb" alt="">
        <h3>{{ product.series }}</h3>
    </div>
</template>
<style scoped>
h3 {
    margin-bottom: 0;
}
</style>