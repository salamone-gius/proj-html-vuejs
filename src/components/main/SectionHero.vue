<template>
    <section class="hero-section">
        <ServicesBar/>
        <JumboTron/>
        <SalesBar/>
    </section>
</template>

<script>
import ServicesBar from './../commons/ServicesBar.vue';
import JumboTron from './../commons/JumboTron.vue';
import SalesBar from './../commons/SalesBar.vue';

export default {
    name: 'SectionHero',

    components: {
        ServicesBar,
        JumboTron,
        SalesBar
    }
}
</script>

<style lang="scss" scoped>

</style>