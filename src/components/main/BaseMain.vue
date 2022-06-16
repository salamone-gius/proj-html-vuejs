<template>
    <main>
        <SectionHero/>
        <SectionCategories/>
    </main>
</template>

<script>
import SectionHero from './SectionHero.vue';
import SectionCategories from './SectionCategories.vue';

export default {
    name: 'BaseMain',

    components: {
        SectionHero,
        SectionCategories,
    }
}
</script>

<style lang="scss" scoped>
</style>