<template>
    <section class="articles-section container">
        <div class="d-flex justify-content-center align-items-center">
            <div class="section-title py-5">
                <h2>Get the best tips & tricks</h2>
                <h5>Recent articles</h5>
            </div>
        </div>
        <ul class="articles row row-cols-4 d-flex justify-content-center mb-5">
            <li class="col">
                <a href="#">
                    <BaseCard
                        :categoryImg="require('../../assets/img/blog-1.jpg')"
                        categoryAlt="Article-1"
                        cardLabel="How to ‘loose leash walk’ your dog"
                        firstPstyle="font-size: 1.50rem; padding: 0 1.5rem; text-align: start; text-align: start;"
                        secondPContentA= "April 21st, 2020"
                        secondPstyle="font-size: 0.875rem; padding: 0 1.5rem; text-align: start;"
                    />
                </a>
            </li>
            <li class="col">
                <a href="#">
                    <BaseCard
                        :categoryImg="require('../../assets/img/blog-2.jpg')"
                        categoryAlt="Article-2"
                        cardLabel="Stop cats from scratching furniture"
                        firstPstyle="font-size: 1.50rem; padding: 0 1.5rem; text-align: start;"
                        secondPContentA= "April 19th, 2020"
                        secondPstyle="font-size: 0.875rem; padding: 0 1.5rem; text-align: start;"
                    />
                </a>
            </li>
            <li class="col">
                <a href="#">
                    <BaseCard
                        :categoryImg="require('../../assets/img/blog-3.jpg')"
                        categoryAlt="Article-3"
                        cardLabel="Where to buy the best pet food"
                        firstPstyle="font-size: 1.50rem; padding: 0 1.5rem; text-align: start;"
                        secondPContentA= "April 18th, 2020"
                        secondPstyle="font-size: 0.875rem; padding: 0 1.5rem; text-align: start;"
                    />
                </a>
            </li>
            <li class="col">
                <a href="#">
                    <BaseCard
                        :categoryImg="require('../../assets/img/blog-4.jpg')"
                        categoryAlt="Article-4"
                        cardLabel="Proper care for your pet toys"
                        firstPstyle="font-size: 1.50rem; padding: 0 1.5rem; text-align: start;"
                        secondPContentA= "April 17th, 2020"
                        secondPstyle="font-size: 0.875rem; padding: 0 1.5rem; text-align: start;"
                    />
                </a>
            </li>
        </ul>
        <div class="button-box">
            <CommonButton
                buttonType="link"
                buttonClass="secondary"
                buttonLink="#"
                buttonText="Read all articles"
            />
        </div>
    </section>
</template>

<script>
import BaseCard from './../commons/BaseCard.vue';
import CommonButton from './../commons/CommonButton.vue';

export default {
    name: 'SectionArticles',

    components: {
        BaseCard,
        CommonButton,
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

    h5 {
        color: var(--tertiary-txt-color);
    }
}

.articles {
    padding: 0;

    li {
        list-style: none;

        a {
            text-decoration: none;
            color: var(--secondary-txt-color);
        }
    }
}

.button-box {
    text-align: center;
    margin-bottom: 6rem;
}
</style>