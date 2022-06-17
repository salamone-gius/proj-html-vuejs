<template>
    <div class="footer-top container">
        <div class="row row-cols-4 d-flex justify-content-between my-5">
            <div class="col">
                <CompanyContacts/>
            </div>
            <div class="col">
                <VerticalNavbar/>
            </div>
        </div>
    </div>
</template>

<script>
import CompanyContacts from './../commons/CompanyContacts.vue';
import VerticalNavbar from './../commons/VerticalNavbar.vue';

export default {
    name: 'FooterTop',

    components: {
        CompanyContacts,
        VerticalNavbar,
    }
}
</script>

<style lang="scss" scoped>
</style>