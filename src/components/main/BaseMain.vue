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
    }
}
</script>

<style lang="scss" scoped>
</style>