<template>
    <div class="base-card">
        <img :src="categoryImg" :alt="categoryAlt">
        <p :style="firstPstyle">{{cardLabel}} {{quantity}}</p>
        <p :class="secondPTag">{{secondPContentA}} {{secondPContentB}}</p>
    </div>
</template>

<script>
export default {
    name: 'BaseCard',

    props: {
        categoryImg: String,
        categoryAlt: String,
        firstPstyle: String,
        cardLabel: String,
        quantity: String,
        secondPTag: String,
        secondPContentA: String,
        secondPContentB: String,

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