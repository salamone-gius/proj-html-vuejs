<template>
    <header>
        <HeaderTop/>
        <HeaderBottom/>
    </header>
</template>

<script>
import HeaderTop from './HeaderTop.vue';
import HeaderBottom from './HeaderBottom.vue';

export default {
    name: 'BaseHeader',

    components: {
        HeaderTop,
        HeaderBottom,
    }
}
</script>

<style lang="scss" scoped>

</style>