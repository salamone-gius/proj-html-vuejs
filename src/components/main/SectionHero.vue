<template>
    <section class="hero-section">
        <ServicesBar/>
        <JumboTron/>
    </section>
</template>

<script>
import ServicesBar from './../commons/ServicesBar.vue';
import JumboTron from './../commons/JumboTron.vue';

export default {
    name: 'SectionHero',

    components: {
        ServicesBar,
        JumboTron,
    }
}
</script>

<style lang="scss" scoped>

</style>