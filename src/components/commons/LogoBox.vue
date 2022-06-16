<template>
    <img :src="logoSrc" :alt="logoAlt">
</template>

<script>
export default {
    name: 'LogoBox',

    props: {
        logoSrc: String,
        logoAlt: String,
    }
}
</script>

<style lang="scss" scoped>

</style>