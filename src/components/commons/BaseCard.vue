<template>
    <div class="base-card">
        <img :src="categoryImg" :alt="categoryAlt">
        <p :style="firstPstyle">{{cardLabel}} {{quantity}}</p>
        <p :style="secondPstyle" :class="secondPTag">
            <span :style="spanStyle">{{spanText}}</span>
            {{secondPContentA}} {{secondPContentB}}
        </p>
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
        spanStyle: String,
        spanText: String,
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

span {
    font-size: .8125rem;
    text-decoration: line-through;
    color: var(--secondary-txt-color);
}

.d-none {
    display: none;
}
</style>