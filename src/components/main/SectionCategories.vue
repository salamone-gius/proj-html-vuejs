<template>
    <section class="categories-section container">
        <div class="d-flex justify-content-center align-items-center">
            <div class="section-title py-5">
                <h2>Browse by category</h2>
                <p>Augue purus et, tincidunt condimentum mauris. At nibh rutrum mi in. Nisi, vitae interdum eleifend dui, consequat nulla rhoncus dictum. Viverra.</p>
            </div>
        </div>
        <ul class="categories row row-cols-4 d-flex justify-content-center mb-5">
            <li class="col">
                <a href="#">
                    <BaseCard
                        :categoryImg="require('../../assets/img/product-9-700x700.jpg')"
                        categoryAlt="Bed"
                        cardLabel="Bed"
                        quantity="(1)"
                    />
                </a>
            </li>
            <li class="col">
                <a href="#">
                    <BaseCard
                        :categoryImg="require('../../assets/img/product-3-700x700.jpg')"
                        categoryAlt="Food"
                        cardLabel="Food"
                        quantity="(6)"
                    />
                </a>
            </li>
            <li class="col">
                <a href="#">
                    <BaseCard
                        :categoryImg="require('../../assets/img/product-2-700x700.jpg')"
                        categoryAlt="Toys"
                        cardLabel="Toys"
                        quantity="(6)"
                    />
                </a>
            </li>
            <li class="col">
                <a href="#">
                    <BaseCard
                        :categoryImg="require('../../assets/img/product-4-700x700.jpg')"
                        categoryAlt="Transport"
                        cardLabel="Transport"
                        quantity="(6)"
                    />
                </a>
            </li>
        </ul>
    </section>
</template>

<script>
import BaseCard from './../commons/BaseCard.vue';

export default {
    name: 'SectionCategories',

    components: {
        BaseCard,
    },
}
</script>

<style lang="scss" scoped>
.section-title {
    width: 50%;
    text-align: center;

    h2 {
        margin-bottom: 1.25rem;
        font-size: 1.875rem;
    }
}

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