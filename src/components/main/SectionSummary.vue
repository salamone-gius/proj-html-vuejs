<template>
    <section class="summary-section">
        <div class="banners d-flex">
            <div class="accessories">
                <img :src="require('../../assets/img/banner-8-2x.jpg')" alt="accessories">
                <div class="claim">
                    <h6>find the best animal supplies</h6>
                    <h2>Popular accessories</h2>
                    <CommonButton
                        buttonType="link"
                        buttonClass="primary"
                        buttonLink="#"
                        buttonText="View all toys accessories"
                    />
                </div>
            </div>
            <div class="food">
                <img :src="require('../../assets/img/banner-9-2x.jpg')" alt="food">
                <div class="claim">
                    <h6>find the best food</h6>
                    <h2>New food arrival</h2>
                    <CommonButton
                        buttonType="link"
                        buttonClass="primary"
                        buttonLink="#"
                        buttonText="View all food products"
                    />
                </div>
            </div>
        </div>
        <div class="services-bar">
            <div class="container d-flex justify-content-between align-items-center py-2">
                <div class="service-1">
                    <i class="fa-solid fa-truck"></i>
                    <div>Free worldwide deliveries</div>
                </div>
                <div class="service-2">
                    <i class="fa-solid fa-map"></i>
                    <div>Find stores near you</div>
                </div>
                <div class="service-3">
                    <i class="fa-solid fa-dollar-sign"></i>
                    <div>Best prices guarranteed </div>
                </div>
                <div class="service-4">
                    <i class="fa-solid fa-credit-card"></i>
                    <div>All credit card accepted</div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import CommonButton from './../commons/CommonButton.vue';

export default {
    name: 'SectionSummary',

    components: {
        CommonButton,
    }
}
</script>

<style lang="scss" scoped>
.summary-section {
    color: var(--primary-txt-color);

    .accessories, .food {
        position: relative;
        width: 50%;
    }

    img {
        width: 100%;
        filter: brightness(55%);
    }

    .claim {
        width: 100%;
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

.services-bar {
    background-color: var(--primary-bg-color);
    background-image: url('../../assets/img/bg-transparent-3.png');
    color: var(--exanary-txt-color);
    text-align: center;

    svg {
        color: var(--primary-txt-color);
        font-size: 2.5rem;
        margin-bottom: 1.5rem;
    }

    .container {
        min-height: 15rem;
    }
}
</style>