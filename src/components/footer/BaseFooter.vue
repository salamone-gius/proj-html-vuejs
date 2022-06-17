<template>
    <footer>
        <FooterTop/>
    </footer>
</template>

<script>
import FooterTop from './FooterTop.vue';

export default {
    name: 'BaseFooter',

    components: {
        FooterTop,
    }
}
</script>

<style lang="scss" scoped>
footer {
    background-color: var(--primary-bg-color);
    color: var(--primary-txt-color);
}
</style>