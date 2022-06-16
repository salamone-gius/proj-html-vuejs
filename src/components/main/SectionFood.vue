<template>
    <section class="food-section container my-5">
        <ul class="categories row row-cols-3 d-flex justify-content-center">
            <li class="col">
                <a href="#">
                    <FoodCard
                        foodBrand="Kibble"
                        foodType="Dry dog food"
                        :foodImg="require('../../assets/img/food-transparent-18.png')"
                        foodAlt="Kibble-food"
                        foodButton="Shop dry food"
                    />
                </a>
            </li>
            <li class="col">
                <a href="#">
                    <FoodCard
                        foodBrand="Moist"
                        foodType="Canned dog food"
                        :foodImg="require('../../assets/img/food-transparent-17.png')"
                        foodAlt="Moist-food"
                        foodButton="Shop moist food"
                    />
                </a>
            </li>
            <li class="col">
                <a href="#">
                    <FoodCard
                        foodBrand="Frozen"
                        foodType="Freeze-Dried dog food"
                        :foodImg="require('../../assets/img/food-transparent-16.png')"
                        foodAlt="Frozen-food"
                        foodButton="Shop frozen food"
                    />
                </a>
            </li>
        </ul>
    </section>
</template>

<script>
import FoodCard from './../commons/FoodCard.vue';

export default {
    name: 'SectionFood',

    components: {
        FoodCard,
    }
}
</script>

<style lang="scss" scoped>
.categories {
    padding: 0;

    li {
        list-style: none;

        a {
            text-decoration: none;
            color: var(--secondary-txt-color);

            &:hover {
                color: var(--tertiary-txt-color);
            }
        }
    }
}

</style>