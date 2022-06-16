<template>
    <div class="header-top">
        <LogoBox :logoSrc="logoInfo.logoImage" :logoAlt="logoInfo.logoImage"/>
    </div>
</template>

<script>
import LogoBox from './../commons/LogoBox.vue';

export default {
    name: 'HeaderTop',

    components: {
        LogoBox,
    },

    data() {
        return {
            logoInfo: {
                logoImage: require('./../../assets/img/dark-pet-logo.png'),
                logoAlt: 'Avada_logo',
            }
        }
    }
}
</script>

<style lang="scss" scoped>

</style>