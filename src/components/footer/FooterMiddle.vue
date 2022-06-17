<template>
    <div class="footer-middle">
        <NavBarBis/>
        <SocialNav/>
    </div>
</template>

<script>
import NavBarBis from './../commons/NavBarBis.vue';
import SocialNav from './../commons/SocialNav.vue';

export default {
    name: 'FooterMiddle',

    components: {
        NavBarBis,
        SocialNav,
    }
}
</script>

<style lang="scss" scoped>

</style>