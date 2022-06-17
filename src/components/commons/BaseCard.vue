<template>
    <div class="base-card">
        <img :src="categoryImg" :alt="categoryAlt">
        <p :style="firstPstyle">{{cardLabel}} {{quantity}}</p>
        <p :style="secondPstyle" :class="secondPTag">{{secondPContentA}} {{secondPContentB}}</p>
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
        secondPstyle: String,
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