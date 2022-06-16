<template>
    <section class="new-arrivals-section container my-5">
        <img :src="require('../../assets/img/banner-3-2x-scaled.jpg')" alt="New-arrivals">
        <div class="claim">
            <h6>find the best animal supplies</h6>
            <h2>New arrivals weekly</h2>
            <CommonButton
                buttonType="link"
                buttonClass="primary"
                buttonLink="#"
                buttonText="Learn more about us"
            />
        </div>
    </section>
</template>

<script>
import CommonButton from './../commons/CommonButton.vue';

export default {
    name: 'SectionNewArrivals',

    components: {
        CommonButton,
    }
}
</script>

<style lang="scss" scoped>
.new-arrivals-section {
    color: var(--primary-txt-color);
    position: relative;

    img {
        width: 100%;
        filter: brightness(55%);
    }

    .claim {
        text-align: center;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);

        h6 {
            text-transform: uppercase;
        }

        h2 {
            margin: 3rem 0;
            font-size: 3.125rem;
        }
    }

}
</style>