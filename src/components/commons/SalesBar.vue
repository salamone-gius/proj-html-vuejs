<template>
    <div class="sales-bar">
        <div class="container d-flex justify-content-center align-items-center pt-4">
            <img :src="require('../../assets/img/food-transparent-5-200x112.png')" alt="On-sale">
            <h3>Get $25 OFF your first purchase of our homemade pet food!</h3>
            <a href="#">Visit the shop</a>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SalesBar',
}
</script>

<style lang="scss" scoped>
.sales-bar {
    background-color: var(--primary-bg-color);
    background-image: url('../../assets/img/bg-transparent-3.png');
    color: var(--primary-txt-color);

    h3, a {
        font-size: 1.25rem;
    }

    h3 {
        margin: 0 2rem;
    }

    a {
        color: var(--exanary-txt-color);

        &:hover {
            color: var(--primary-txt-color);
        }
    }

}
</style>