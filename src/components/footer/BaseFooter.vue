<template>
    <footer>
        <FooterTop/>
        <FooterMiddle/>
    </footer>
</template>

<script>
import FooterTop from './FooterTop.vue';
import FooterMiddle from './FooterMiddle.vue';

export default {
    name: 'BaseFooter',

    components: {
        FooterTop,
        FooterMiddle,
    }
}
</script>

<style lang="scss" scoped>
footer {
    background-color: var(--primary-bg-color);
    color: var(--primary-txt-color);
}
</style>