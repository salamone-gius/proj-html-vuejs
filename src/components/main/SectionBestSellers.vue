<template>
    <section class="best-sellers-section container">
        <div class="d-flex justify-content-between align-items-center">
            <div class="section-title py-5">
                <h6>All-time best sellers</h6>
                <h2>Items everyone loves</h2>
            </div>
            <div class="button">
                <CommonButton
                    buttonType="link"
                    buttonClass="secondary"
                    buttonLink="#"
                    buttonText="View all products"
                />
            </div>
        </div>
        <ul class="items row row-cols-4 d-flex justify-content-center mb-5">
            <li class="col">
                <a href="#">
                    <BaseCard
                        :categoryImg="require('../../assets/img/product-21-800x800.jpg')"
                        categoryAlt="Transport cage"
                        firstPstyle="font-size: 1.375rem;"
                        cardLabel="Transport cage"
                        secondPContentA="$ 25.00"
                        secondPstyle="color: var(--tertiary-txt-color);"
                    />
                </a>
            </li>
            <li class="col">
                <a href="#">
                    <BaseCard
                        :categoryImg="require('../../assets/img/product-20-800x800.jpg')"
                        categoryAlt="Dog leash"
                        firstPstyle="font-size: 1.375rem;"
                        cardLabel="Dog leash"
                        secondPContentA="$ 25.00"
                        secondPstyle="color: var(--tertiary-txt-color);"
                    />
                </a>
            </li>
            <li class="col">
                <a href="#">
                    <BaseCard
                        :categoryImg="require('../../assets/img/product-16-800x800.jpg')"
                        categoryAlt="Animal transport cage"
                        firstPstyle="font-size: 1.375rem;"
                        cardLabel="Animal transport cage"
                        secondPContentA="$ 25.00"
                        secondPstyle="color: var(--tertiary-txt-color);"
                        spanText="$ 35.00"
                    />
                </a>
            </li>
            <li class="col">
                <a href="#">
                    <BaseCard
                        :categoryImg="require('../../assets/img/product-11-800x800.jpg')"
                        categoryAlt="Colorful cat leash"
                        firstPstyle="font-size: 1.375rem;"
                        cardLabel="Colorful cat leash"
                        secondPContentA="$ 12.00"
                        secondPstyle="color: var(--tertiary-txt-color);"
                    />
                </a>
            </li>
        </ul>
    </section>
</template>

<script>
import CommonButton from './../commons/CommonButton.vue';
import BaseCard from './../commons/BaseCard.vue';

export default {
    name: 'SectionBestSellers',

    components: {
        CommonButton,
        BaseCard,
    }
}
</script>

<style lang="scss" scoped>
.section-title {
    h2 {
        margin-top: 1.25rem;
        font-size: 1.875rem;
        color: var(--secondary-txt-color);
    }

    h6 {
        color: var(--tertiary-txt-color);
        font-size: 1.25rem;
    }

}

.items {
    padding: 0;

    li {
        list-style: none;

        a {
            text-decoration: none;
            color: var(--secondary-txt-color);
        }
    }
}
</style>