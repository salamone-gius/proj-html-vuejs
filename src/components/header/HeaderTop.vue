<template>
    <div class="header-top">
        <div class="logo-box">
            <LogoBox :logoSrc="logoInfo.logoImage" :logoAlt="logoInfo.logoImage"/>
        </div>
        <div class="searchbar">
            <SearchBar/>
        </div>
    </div>
</template>

<script>
import LogoBox from './../commons/LogoBox.vue';
import SearchBar from './../commons/SearchBar.vue';

export default {
    name: 'HeaderTop',

    components: {
        LogoBox,
        SearchBar,
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