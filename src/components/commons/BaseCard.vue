<template>
    <div class="base-card">
        <img :src="categoryImg" :alt="categoryAlt">
        <p>{{cardLabel}} {{quantity}}</p>
        <p :class="secondPTag">{{secondPContent}}</p>
    </div>
</template>


// require('../../assets/img/product-9-300x300.jpg')


<script>
export default {
    name: 'BaseCard',

    props: {
        categoryImg: String,
        categoryAlt: String,
        cardLabel: String,
        quantity: String,
        secondPTag: String,
        secondPContent: String,
    }
}
</script>

<style lang="scss" scoped>
img {
    width: 100%;
}

p {
    text-align: center;
    margin-top: 1rem;
}

.d-none {
    display: none;
}
</style>