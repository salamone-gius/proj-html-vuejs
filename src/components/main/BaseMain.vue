<template>
    <main>
        <SectionHero/>
        <SectionCategories/>
        <SectionFood/>
        <SectionNewArrivals/>
        <SectionBestSellers/>
        <SectionUsersTestimonials/>
        <SectionNewsletter/>
        <SectionArticles/>
        <SectionSummary/>
        <SectionNewProducts/>
    </main>
</template>

<script>
import SectionHero from './SectionHero.vue';
import SectionCategories from './SectionCategories.vue';
import SectionFood from './SectionFood.vue';
import SectionNewArrivals from './SectionNewArrivals.vue';
import SectionBestSellers from './SectionBestSellers.vue';
import SectionUsersTestimonials from './SectionUsersTestimonials.vue';
import SectionNewsletter from './SectionNewsletter.vue';
import SectionArticles from './SectionArticles.vue';
import SectionSummary from './SectionSummary.vue';
import SectionNewProducts from './SectionNewProducts.vue';

export default {
    name: 'BaseMain',

    components: {
        SectionHero,
        SectionCategories,
        SectionFood,
        SectionNewArrivals,
        SectionBestSellers,
        SectionUsersTestimonials,
        SectionNewsletter,
        SectionArticles,
        SectionSummary,
        SectionNewProducts,
    }
}
</script>

<style lang="scss" scoped>
</style>