<template>
    <div class="food-card">
        <div class="card-title">
            <h2>{{foodBrand}}</h2>
            <h4>{{foodType}}</h4>
        </div>
        <img :src="foodImg" :alt="foodAlt">
        <CommonButton
            buttonType="link"
            buttonClass="secondary"
            buttonLink="#"
            :buttonText="foodButton"
        />
    </div>
</template>

<script>
import CommonButton from './CommonButton.vue';

export default {
    name: 'FoodCard',

    components: {
        CommonButton,
    },

    props: {
        foodBrand: String,
        foodType: String,
        foodImg: String,
        foodAlt: String,
        foodButton: String,
    }
}
</script>

<style lang="scss" scoped>
.food-card {
    background-color: var(--primary-bg-color);
    cursor: pointer;
    transition: transform 1s;
    padding-bottom: 3rem;
    text-align: center;

    &:hover {
        transform: scale(1.1);
        filter: brightness(1.1);
    }

    .card-title {
        background-image: url('../../assets/img/bg-transparent-3.png');

        h2 {
            color: var(--primary-txt-color);
            padding-top: 3rem;
        }

        h4 {
            color: var(--tertiary-txt-color);
            padding: 1rem 0;
        }
    }
    img {
        width: 100%;
        padding: 1rem;
    }
}
</style>