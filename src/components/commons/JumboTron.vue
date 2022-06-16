<template>
    <div class="jumbotron">
        <img :src="require('../../assets/img/banner-5-2x-scaled.jpg')" alt="Hero-image">
        <div class="claim">
            <h6>find the best animal supplies</h6>
            <h1>We know animals are a part of your family, let us help take care of them.</h1>
            <CommonButton
                buttonType="link"
                buttonClass="primary"
                buttonLink="#"
                buttonText="Learn more about us"
            />
        </div>
    </div>
</template>

<script>
import CommonButton from './CommonButton.vue';

export default {
    name: 'JumboTron',

    components: {
        CommonButton,
    }
}
</script>

<style lang="scss" scoped>
.jumbotron {
    color: var(--primary-txt-color);
    position: relative;

    img {
        width: 100%;
    }

    .claim {
        position: absolute;
        top: 50%;
        left: 6rem;
        transform: translateY(-50%);
        width: 40%;   


        h6 {
            text-transform: uppercase;
        }

        h1 {
            margin: 3rem 0;
            font-size: 3.125rem;
        }
    }

}

</style>