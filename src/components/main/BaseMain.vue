<template>
    <main>
        <SectionHero/>
        <SectionCategories/>
        <SectionFood/>
        <SectionNewArrivals/>
        <SectionBestSellers/>
        <SectionUsersTestimonials/>
        <SectionNewsletter/>
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
    }
}
</script>

<style lang="scss" scoped>
</style>