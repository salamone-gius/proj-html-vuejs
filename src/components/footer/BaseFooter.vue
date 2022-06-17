<template>
    <footer>
        <FooterTop/>
        <FooterMiddle/>
        <FooterBottom/>
    </footer>
</template>

<script>
import FooterTop from './FooterTop.vue';
import FooterMiddle from './FooterMiddle.vue';
import FooterBottom from './FooterBottom.vue';

export default {
    name: 'BaseFooter',

    components: {
        FooterTop,
        FooterMiddle,
        FooterBottom,
    }
}
</script>

<style lang="scss" scoped>
footer {
    background-color: var(--primary-bg-color);
    color: var(--primary-txt-color);
}
</style>