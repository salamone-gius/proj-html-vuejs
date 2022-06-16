<template>
    <main>
        <SectionHero/>
        <SectionCategories/>
        <SectionFood/>
        <SectionNewArrivals/>
    </main>
</template>

<script>
import SectionHero from './SectionHero.vue';
import SectionCategories from './SectionCategories.vue';
import SectionFood from './SectionFood.vue';
import SectionNewArrivals from './SectionNewArrivals.vue';

export default {
    name: 'BaseMain',

    components: {
        SectionHero,
        SectionCategories,
        SectionFood,
        SectionNewArrivals,
    }
}
</script>

<style lang="scss" scoped>
</style>