<template>
    <main>
        <SectionHero/>
        <SectionCategories/>
        <SectionFood/>
        <SectionNewArrivals/>
        <SectionBestSellers/>
    </main>
</template>

<script>
import SectionHero from './SectionHero.vue';
import SectionCategories from './SectionCategories.vue';
import SectionFood from './SectionFood.vue';
import SectionNewArrivals from './SectionNewArrivals.vue';
import SectionBestSellers from './SectionBestSellers.vue';

export default {
    name: 'BaseMain',

    components: {
        SectionHero,
        SectionCategories,
        SectionFood,
        SectionNewArrivals,
        SectionBestSellers,
    }
}
</script>

<style lang="scss" scoped>
</style>