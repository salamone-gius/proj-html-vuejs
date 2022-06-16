<template>
    <div class="header-top container d-flex justify-content-between align-items-center py-2">
        <div class="logo-box">
            <LogoBox :logoSrc="logoInfo.logoImage" :logoAlt="logoInfo.logoImage"/>
        </div>
        <div class="searchbar">
            <SearchBar/>
        </div>
        <div class="contact-us">
            <ContactUs/>
        </div>
        <div class="header-icons">
            <HeaderIcons/>
        </div>
    </div>
</template>

<script>
import LogoBox from './../commons/LogoBox.vue';
import SearchBar from './../commons/SearchBar.vue';
import ContactUs from './../commons/ContactUs.vue';
import HeaderIcons from './../commons/HeaderIcons.vue';

export default {
    name: 'HeaderTop',

    components: {
        LogoBox,
        SearchBar,
        ContactUs,
        HeaderIcons,
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