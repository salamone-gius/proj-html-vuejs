<template>
    <section class="new-products-section py-5">
        <div class="d-flex justify-content-center align-items-center">
            <div class="section-title py-5">
                <h2>New products arrival</h2>
                <h5>Latest products</h5>
            </div>
        </div>
        <div class="products container">
            <ul class="items row row-cols-3 d-flex justify-content-between">
                <li class="col">
                    <a href="#">
                        <BaseCard
                            :categoryImg="require('../../assets/img/product-8.jpg')"
                            categoryAlt="Colored pet bed"
                            firstPstyle="font-size: 1.375rem;"
                            cardLabel="Colored pet bed"
                            secondPContentA="$18.00 - $ 26.00"
                            secondPstyle="color: var(--tertiary-txt-color);"
                        />
                    </a>
                </li>
                <li class="col">
                    <a href="#">
                        <BaseCard
                            :categoryImg="require('../../assets/img/product-2.jpg')"
                            categoryAlt="Colorful ball set"
                            firstPstyle="font-size: 1.375rem;"
                            cardLabel="Colorful ball set"
                            secondPContentA="$ 29.00"
                            secondPstyle="color: var(--tertiary-txt-color);"
                        />
                    </a>
                </li>
                <li class="col">
                    <a href="#">
                        <BaseCard
                            :categoryImg="require('../../assets/img/product-3.jpg')"
                            categoryAlt="Dog bone"
                            firstPstyle="font-size: 1.375rem;"
                            cardLabel="Dog bone"
                            secondPContentA="$ 18.00"
                            secondPstyle="color: var(--tertiary-txt-color);"
                        />
                    </a>
                </li>
            </ul>
            <ul class="items row row-cols-3 d-flex justify-content-between mb-5">
                <li class="col">
                    <a href="#">
                        <BaseCard
                            :categoryImg="require('../../assets/img/product-4.jpg')"
                            categoryAlt="Animal transport bag"
                            firstPstyle="font-size: 1.375rem;"
                            cardLabel="Animal transport bag"
                            secondPContentA="$ 29.00"
                            secondPstyle="color: var(--tertiary-txt-color);"
                        />
                    </a>
                </li>
                <li class="col">
                    <a href="#">
                        <BaseCard
                            :categoryImg="require('../../assets/img/product-5.jpg')"
                            categoryAlt="Animal transport cage"
                            firstPstyle="font-size: 1.375rem;"
                            cardLabel="Animal transport cage"
                            secondPContentA="$ 35.00"
                            secondPstyle="color: var(--tertiary-txt-color);"
                        />
                    </a>
                </li>
                <li class="col">
                    <a href="#">
                        <BaseCard
                            :categoryImg="require('../../assets/img/product-10.jpg')"
                            categoryAlt="Closable cat litter"
                            firstPstyle="font-size: 1.375rem;"
                            cardLabel="Closable cat litter"
                            secondPContentA="$ 16.00"
                            secondPstyle="color: var(--tertiary-txt-color);"
                        />
                    </a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
import BaseCard from './../commons/BaseCard.vue';

export default {
    name: 'SectionNewProducts',

    components: {
        BaseCard,
    }
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

    h5 {
        color: var(--tertiary-txt-color);
    }
}

.products {
    ul {
        padding: 0;
    }

    li {
        list-style: none;

        a {
            text-decoration: none;
            color: var(--secondary-txt-color);
        }
    }
}

</style>