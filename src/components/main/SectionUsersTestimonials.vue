<template>
    <section class="users-testimonials-section">
        <div class="section-title">
            <h2>Users Testimonials</h2>
        </div>
        <div class="section-cards container">
            <div class="row row-cols-3 d-flex justify-content-between">
                <div class="col">
                    <TestimonialsCard
                        :cardImg="require('../../assets/img/avatar-3.jpg')"
                        cardAlt="Lisa Smith"
                        firstCardTxt="Auctor est habitasse amet nunc, interdum vel mattis sodales cras. Ut nulla quis nunc, tincidunt eu. Eu."
                        secondCardTxt="Lisa Smith, ThemeFusion"
                    />
                </div>
                <div class="col">
                    <TestimonialsCard
                        :cardImg="require('../../assets/img/avatar-1.jpg')"
                        cardAlt="Melissa Green"
                        firstCardTxt="Donec sollicitudin molestie malesuada. Vivamus suscipit tortor eget felis porttitor volutpat vestibulum ac diam sit."
                        secondCardTxt="Melissa Green, ThemeFusion"
                    />
                </div>
                <div class="col">
                    <TestimonialsCard
                        :cardImg="require('../../assets/img/avatar-4.jpg')"
                        cardAlt="Sam Lewis"
                        firstCardTxt="Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem. Proin eget tortor risus vestibulum ante ipsum."
                        secondCardTxt="Sam Lewis, ThemeFusion"
                    />
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import TestimonialsCard from './../commons/TestimonialsCard.vue';

export default {
    name: 'SectionUsersTestimonials',

    components: {
        TestimonialsCard,
    }
}
</script>

<style lang="scss" scoped>
.users-testimonials-section {
    background-color: var(--primary-bg-color);
    color: var(--primary-txt-color);
    padding-bottom: 8rem;

    .section-title {
        background-image: url('../../assets/img/bg-transparent-3.png');
        padding: 4rem;

        h2 {
            font-size: 2rem;
            text-align: center;
        }
    }
}
</style>