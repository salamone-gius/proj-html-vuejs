<template>
    <div class="services-bar">
        <div class="container d-flex justify-content-around py-3">
            <div class="service-1">
                <i class="fa-regular fa-map"></i>
                <span class="highlighted">International </span>
                <span>Shipping Services</span>
            </div>
            <div class="service-2">
                <i class="fa-regular fa-clock"></i>
                <span>See our </span>
                <span class="highlighted">store hours </span>
                <span>and services</span>
            </div>
            <div class="services-3">
                <i class="fa-solid fa-check"></i>
                <span>We price match to give you the </span>
                <span class="highlighted">best deals</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ServicesBar',
}
</script>

<style lang="scss" scoped>
.services-bar {
    background-color: var(--primary-bg-color);
    background-image: url('../../assets/img/bg-transparent-3.png');
    color: var(--exanary-txt-color);

    svg, .highlighted {
        color: var(--primary-txt-color);
    }

    svg {
        margin-right: .625rem;
        vertical-align: middle;
    }
}
</style>