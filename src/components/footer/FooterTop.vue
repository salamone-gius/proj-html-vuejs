<template>
    <div class="footer-top container">
        <div class="row row-cols-4 d-flex justify-content-between my-5">
            <div class="col">
                <CompanyContacts/>
            </div>
            <div class="col">
                <VerticalNavbar/>
            </div>
            <div class="col">
                <VerticalNavbarBis/>
            </div>
            <div class="col subscribe">
                <h5>Subscribe to our newsletter</h5>
                <div class="subscrive-form">
                    <SubscribeForm
                        inputStyle="width: 12rem;"
                    />
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import CompanyContacts from './../commons/CompanyContacts.vue';
import VerticalNavbar from './../commons/VerticalNavbar.vue';
import VerticalNavbarBis from './../commons/VerticalNavbarBis.vue';
import SubscribeForm from './../commons/SubscribeForm.vue';

export default {
    name: 'FooterTop',

    components: {
        CompanyContacts,
        VerticalNavbar,
        VerticalNavbarBis,
        SubscribeForm,
    }
}
</script>

<style lang="scss" scoped>
.footer-top {
    border-bottom: 1px solid var(--quaternary-txt-color);
    padding-top: 3rem;

    .subscribe {
        background-color: var(--eptenary-bg-color);
        background-image: url('../../assets/img/bg-transparent-3.png');
        padding: 2rem;

        h5 {
            margin-bottom: 1.25rem;
        }
    }
}
</style>