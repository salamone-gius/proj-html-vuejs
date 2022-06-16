<template>
    <main>
        <SectionHero/>
        <SectionCategories/>
        <SectionFood/>
    </main>
</template>

<script>
import SectionHero from './SectionHero.vue';
import SectionCategories from './SectionCategories.vue';
import SectionFood from './SectionFood.vue';

export default {
    name: 'BaseMain',

    components: {
        SectionHero,
        SectionCategories,
        SectionFood,
    }
}
</script>

<style lang="scss" scoped>
</style>